# How can we add additional features to the protocol without breaking previous functionality?
  
   Each new version of the protocol should have a unique version number. The version number should be included in the header of each card, so that receivers can determine which version of the protocol is being used. And to allow for any kind of extension we can imagine, we should introduce an extension mechanism that allows new fields to be added to the header of the card. Each extension field should have a some sort of a way to uniquely identify it , and should have a descriptions of its purpose and usage.

# Send to any individual on the whole UW campus
  To send a card to any individual on the whole UW campus, we can add an extension ID that specifies the recipient's ID or email address. Nodes that receive a card with this extension ID should forward the card to the specified recipient.
# Specify whether contents are ASCII text, Unicode text, or binary values
  We can add an extension ID that specifies the data type. Nodes that receive a card with this extension ID should handle the contents of the card accordingly.
# Keep a record of what nodes the card has passed through.
  We can add an extension ID that specifies a list of node IDs. Each node that receives the card should add its own ID to the list before forwarding the card. Nodes that receive a card with this extension ID should update the list of node IDs and forward the card to the next node.
