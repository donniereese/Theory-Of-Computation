# Car Lights Turn Signal

```
+------------+
| Engine Off |
+------------+
   |
   |
   [ Powered On ]
   |                   
   V                  |#|                                     |#|
+-------+            +--------------------+        +-------------+              
| Start |            | Turn Signal Switch |        |   Hazzard   |              
| Power |            |      Position      |        | Switch Pos. |              
+-------+            +--------------------+        +-------------+              
   |                 |           |       |         |                                                          
   |                 |           |       |         |                                                          
   |                 |           |       |         +----------+                                                    
   +-----------------|-----+-----|-------|---------| Disabled |                                                     
   |                 |     |     |       |         +----------+
   |                 |     V     |       |         |                         
   |                 +-------------------+         [ Powered ]                                                
   |                 |     Disabled      |         |                                                    
   |                 +-------------------+         V                                                          
   |                 |           |       |         +--------+
   |                 |           |       |         | Active |---+
   |        +-[ ε ]--+--+        |       |         +--------+   |
   |        |           |        |       |                      [ Switched On ]
   |        |           |        |       |                      |
   |        |           |        |       |                      |
   |        |       [ ε ]        |       |                      |
   |        |           |        |       |                      |
   |        V           |        |       |                      |
   |   +----------+     •        •       •    +--------+        | +----+                       +-------+
   +---| Disabled |>--[ Powered Supplied ]--> | Active |---+    +-| On |-----------------------| Blink |-----> Light
   |   +----------+     •        •       •    +--------+   |    | +----+                       +-------+
   |                    |        |       |                 |    |                                  ^ 
   |                    |        |       |                 |    |       +-----+                    | 
   |        +-----------+        |       |                 +----|-------| Off |---[ On ]-----------+     
   |        |                    |       |                      |       +-----+                      
   |        |                    |       |                      |          ^                          
   |        |                    |       |                      |          |                        
   |        |                    |       +-----[ Switched On ]--|----------+                          
   |        V                    |                              |                                     
   |   +----------+              •            +--------+        | +----+                                
   +---| Disabled |>--[ Powered Supplied ]--> | Active |---+    +-| On |---------------------------+
       +----------+              •            +--------+   |      +----+                           |  
                                 |                         |                                       V     
                                 |                         |            +-----+                +-------+
                                 |                         +------------| Off |---[ On ]-------| Blink |-----> Light
                                 |                                      +-----+                +-------+
                                 |                                         ^
                                 |                                         |
                                 +--------------------[ Switched On ]------+

```