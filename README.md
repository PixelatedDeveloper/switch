# In-depth on Nintendo Switch games
Making a list of games, their resolutions in different modes, framerates and other noteworthy things.

# Helping me out
In case you want to help this fun little open-source project out you can do a pull request with your game additions to the '_data/games.yaml' file or other relevant improvements. 

## Format
Required example baseformat is as follows:

    - name: Sonic Mania
      handheld: "720p"
      docked: "1080p"
      fps: 60fps

It's also allowed to use a 'from-to' like statement for the resolutions when dynamic scaling is active (see item below). For example:

      handheld: "600p-720p"
      docked: "900p-1080p"

### Optional items
Dynamic resolution scaling
To add the dynamic resolution scaling, add the following item to the baseformat

      dynamic_scaling: true

Verified items
Verified items are basically stats that are verified by either their creators (twitter), news articles/interviews or other sources like DigitalFoundry. To add a verified item first add the status:

      verified_status: true

And after that add the URL:

      verified_url: "https://switchgame.com/specs.html"

Notes
To add a note to a item for example mentioning a specific framerate for a mode (MP=60fps, SP=30fps) can be done through the notes item.

      notes: "Handheld framerate drops to 20fps"

### Complete format
The complete format with all in place should look like:

    - name: Sonic Mania
      handheld: "600p-720p"
      docked: "1080p"
      fps: 60fps
      dynamic_scaling: true
      verified_status: true
      verified_url: "https://switchgame.com/specs.html"