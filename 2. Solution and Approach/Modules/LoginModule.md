# Login Module

Login module (displayed on [Conceptual Design](../ConceptualDesign) in some <text style="color:lightgreen;">Green</text> Box) is used for authenticating users before allowing them to enter any of StayHealthy Inc.'s MonitorMe application.

Authentication is processed using OpenID Connect (OIDC), an authentication layer built on the Open Authorization (OAuth) standard protocol. 
Authentication is done by starting with user credentials. After getting user credentials, next step is processing it over an *encryption* or one-way hashing function, followed by addition of a unique and private *salt* content to the encrypted output and then comparing this processed value with such an existing registration record for the access key of the submitted username. 

This process helps in keeping the original sensitive authentication information secured from cases such as outer network eavesdropping or when any part of the database records get compromised.