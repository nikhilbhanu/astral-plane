# Astral Plane

Astral Plane is an intelligent system that employs Ambisonics to enable audio spatialization for live performances, especially with Ableton Live.

  - Object audio (each track in Live is a Sound Object.)
  - Synced up with Live using Ableton Link.
  - Control object positions and movement patterns using OSC.
  - Extracts audio features to create interesting mappings based on audio content (coming soon!)

# Prerequisites
  - Ableton Live 9.6+
  - Max 7
  - Soundflower v 2.0b2
  - HOALibrary for Max (https://github.com/CICM/HoaLibrary-Max). Place the package folder in the Max packages folder. (What a phenomenal library, kudos to these guys!)

# Setup
  - Set the audio output in Ableton to Soundflower (64ch)
  - Set the audio input in Max to Soundflower (64ch)
  - The audio objects are sequentially arranged, therefore choose the output of each track in Live accordingly (As of now 4 channels). For example, set track 1 to output to channel 1 and it assigns it as the first sound object.
  - Switch on Link.
  - If you're a Lemur user, you can use the the patch provided. (set your IP in the app and set the port to 7001.)
  - Open AstralPlane.maxpat

# Use
  - The system can be used with any application capable of transmitting OSC. The routes can be found in the AstralPlane.Control.maxpat. I use it with Lemur.
  - For testing purposes, there are controls provided in the patch.

# Trajectories & Rate
  - There are two trajectories implemented as of now, Ellipse and Lissajous curve.
  - User can set the origin of an object and the object will move in selected trajectories about that origin.
  - User can adjust parameters to get different curves (a, b, magnitude).
  - There are three Sync Modes Bar, Beat (sub-divions of Bar) and Free.

# Stay tuned, more features coming soon!
