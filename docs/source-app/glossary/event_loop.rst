.. _event_loop:

##########
Event loop
##########

Drawing inspiration from modern web frameworks like `React.js <https://reactjs.org/>`_, the Lightning app runs all flows in an **event loop** (forever), which is triggered several times a second after collecting any works' state change.

.. figure::  https://pl-flash-data.s3.amazonaws.com/assets_lightning/lightning_loop.gif

When running an app in the cloud, the ``LightningWork`` run on different machines. LightningWork communicates any state changes to the **event loop** which re-executes the flow with the newly-collected works' state.
