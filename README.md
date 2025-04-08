# Config for Totem with Dongle Display

Notes:
- &kp = key press
- &trans = transparent
- &lt = layer toggle
- &mt = modifier toggle
- &bootloader = bootloader
- &to = to layer
- &studio_unlock = studio unlock

Thumb clusters will be fixed to 
|ESC|TAB|SPC| |RET|BSP|DEL|

Layers:
- Basetap```
  - Q W E R T   Y U I O P
  - A S D F G   H J K L ;
  - Z X C V B   N M , . /
```
- BaseHold```
  - Layer1 Layer2 Layer3 Layer4 Layer5 YUIOP
  - Layer6 Layer7 Layer8 Layer9 Layer0 HJKL;
  - LSHIFT LCTRL  LSUPER LALT          RALT RSUPER RCTRL RSHIFT   
```
- Num```
  -      +789-
  -      *456/
  -      0123.
```
- Sym```
  -      [&~#]
  -      {$%^}
  -      (!"£)    
```
- Fun
- Game
- Gameplus
- Spare1
- Spare2
- Spare3
- Config

Added extra spare layers

        Base {            
            display-name = "Base";
            bindings = <
            // top Row
              &kp Q       
              &kp W       
              &kp E          
              &kp R         
              &kp T        
              &kp Y    
              &kp U        
              &kp I        
              &kp O       
              &kp P

            // middle Row
              &hm LGUI A  
              &hm LALT S  
              &hm LCTRL D    
              &hm LSHIFT F  
              &kp G        
              &kp H    
              &hm RSHFT J  
              &hm RCTRL K  
              &hm RALT L  
              &hm RGUI SEMICOLON

            // bottom Row
              &lt 3 ESCAPE  
              &kp Z       
              &kp X       
              &kp C          
              &kp V         
              &kp B        
              &kp N    
              &kp M        
              &kp COMMA    
              &kp DOT     
              &kp SLASH           
              &kp APOSTROPHE

            // Thumb Row
              &mt LCTRL DEL  
              &lt 1 TAB     
              &kp SPACE    
              &kp RET  
              &lt 2 BSPC   
              &kp MINUS
            >;
        };
