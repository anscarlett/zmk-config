//
//                                                        ▀▀▀▀▀     ▀▀▀▀▀          ▀▀█▀▀
//                                                        ▄▀▀▀▄  ▄  ▄▀▀▀▄  ▄  ▄▀▀▀▄  █  ▄▀▀▀▄
//                                                        █   █  █  █   █  █  █   █  █  █   █
//                                                         ▀▀▀   █   ▀▀▀   █   ▀▀▀   ▀   ▀▀▀
//                                                               █      ▄▄▄█▄▄▄    █   █  
//                                                               ▀      █  █  █     █▄█
//                                                             ▀▀▀▀▀    █  █  █      ▀
//                                                                      ▀  ▀  ▀
//
// ▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄

#include <behaviors.dtsi>
#include <dt-bindings/zmk/keys.h>

#define Base        0
#define Num         1
#define Sym         2
#define Fun         3
#define Game        4
#define Gameplus    5
#define Spare1      6
#define Spare2      7
#define Spare3      8
#define Config      9

&mt {
    quick-tap-ms = <100>;
    global-quick-tap;
    flavor = "tap-preferred";
    tapping-term-ms = <170>;
};

&lt {
    tapping-term-ms = <240>;
    flavor = "balanced";
    quick-tap-ms = <150>;
};

/ {
    behaviors {
        hm: homerow_mods {
            compatible = "zmk,behavior-hold-tap";
            label = "HOMEROW_MODS";
            #binding-cells = <2>;
            flavor = "tap-preferred";
            tapping-term-ms = <200>;
            quick-tap-ms = <125>;
            global-quick-tap;
            bindings = <&kp>, <&kp>;
        };                            
    };

    keymap {
        compatible = "zmk,keymap";

        Base {
            display-name = "Base";
            bindings = <
              &mo 1 Q
              &mo 2 W
              &mo 3 E          
              &mo 4 R         
              &mo 5 T        
              &kp Y    
              &kp U        
              &kp I        
              &kp O       
              &kp P

              &mo 6 A       
              &mo 7 S       
              &mo 8 D          
              &mo 9 F  
              &kp G        
              &kp H    
              &kp J  
              &kp K  
              &kp L  
              &kp SEMICOLON

              &trans  
              &hm LSHIFT Z  
              &hm LCTRL X   
              &hm LGUI C       
              &hm LALT V         
              &kp B        
              &kp N    
              &hm RALT M        
              &hm RGUI COMMA    
              &hm RCTRL DOT     
              &hm RSHIFT SLASH           
              &trans

              &kp ESC  
              &kp TAB     
              &kp SPACE    
              &kp RET  
              &kp BSPC   
              &kp DEL
            >;
        };

        Num {
            display-name = "Num";
            bindings = <
              &kp AT       
              &kp AT     
              &kp AT  
              &kp AT     
              &kp AT    
              &kp SLASH
              &kp NUMBER_8  
              &kp NUMBER_9  
              &kp ASTERISK

              &kp AT  
              &kp AT   
              &kp AT      
              &kp AT  
              &kp AT    
              &kp MINUS  
              &kp NUMBER_4  
              &kp NUMBER_5  
              &kp NUMBER_6  
              &kp PLUS
              
              &trans 
              &kp AT    
              &kp AT  
              &kp AT        
              &kp AT   
              &kp AT    
              &kp NUMBER_0  
              &kp NUMBER_1  
              &kp NUMBER_2  
              &kp NUMBER_3  
              &kp DOT  
              &trans
              
              &trans        
              &trans     
              &trans      
              &trans    
              &trans        
              &trans

            >;
        };

        Sym {
            display-name = "Sym";
            bindings = <
                &kp EXCL  &kp AT  &kp HASH  &kp DOLLAR  &kp PERCENT    &kp CARET  &kp AMPERSAND  &kp KP_ASTERISK  &kp SQT  &kp DQT
                &trans    &trans  &trans    &trans      &trans         &trans     &trans         &trans           &trans   &trans
&studio_unlock  &trans    &trans  &trans    &trans      &trans         &kp UNDER  &kp EQUAL      &trans           &trans   &kp SLASH  &kp HOME
                                  &trans    &trans      &trans         &trans     &trans         &trans
            >;
        };

        Fun {
            display-name = "Fun";
            bindings = <
        &bootloader  &trans  &trans  &trans  &to 4     &trans  &trans  &trans  &kp END  &kp F1
        &trans       &trans  &trans  &trans  &trans    &trans  &trans  &trans  &trans   &kp F10
&trans  &trans       &trans  &trans  &trans  &trans    &trans  &trans  &trans  &trans   &kp F20  &kp F7
                             &trans  &trans  &trans    &trans  &trans  &trans
            >;
        };

        Gaming {
            display-name = "Game";
            bindings = <
            &kp Z           &kp X  &kp C      &kp V         &sl 5     &trans  &trans  &trans  &trans  &trans
            &kp TAB         &kp Q  &kp W      &kp E         &kp R     &trans  &trans  &trans  &trans  &trans
&kp ESCAPE  &kp LEFT_SHIFT  &kp A  &kp S      &kp D         &kp F     &trans  &trans  &trans  &trans  &trans  &trans
                                   &kp LCTRL  &kp LEFT_ALT  &trans    &trans  &trans  &trans
            >;
        };

        Gaming+ {
            display-name = "Game+";
            bindings = <
        &kp F10  &kp NUMBER_1  &kp NUMBER_2  &kp NUMBER_3  &kp T     &kp RA(RC(Y))  &kp RA(RC(U))  &trans  &trans  &kp LC(RA(DEL))
        &kp L    &kp O         &kp Y         &kp K         &kp G     &kp F5         &trans         &trans  &trans  &trans
&trans  &to 0    &trans        &trans        &trans        &trans    &trans         &trans         &trans  &trans  &trans           &kp LA(F4)
                               &kp J         &kp I         &kp M     &trans         &trans         &trans
            >;
        };
        Spare1 {
            display-name = "Spare1";
            bindings = <
        &bootloader  &trans  &trans  &trans  &to 4     &trans  &trans  &trans  &kp END  &kp F1
        &trans       &trans  &trans  &trans  &trans    &trans  &trans  &trans  &trans   &kp F10
&trans  &trans       &trans  &trans  &trans  &trans    &trans  &trans  &trans  &trans   &kp F20  &kp F7
                             &trans  &trans  &trans    &trans  &trans  &trans
            >;
        };
        Spare2 {
            display-name = "Spare2";
            bindings = <
        &bootloader  &trans  &trans  &trans  &to 4     &trans  &trans  &trans  &kp END  &kp F1
        &trans       &trans  &trans  &trans  &trans    &trans  &trans  &trans  &trans   &kp F10
&trans  &trans       &trans  &trans  &trans  &trans    &trans  &trans  &trans  &trans   &kp F20  &kp F7
                             &trans  &trans  &trans    &trans  &trans  &trans
            >;
        };
        Spare3 {
            display-name = "Spare3";
            bindings = <
        &bootloader  &trans  &trans  &trans  &to 4     &trans  &trans  &trans  &kp END  &kp F1
        &trans       &trans  &trans  &trans  &trans    &trans  &trans  &trans  &trans   &kp F10
&trans  &trans       &trans  &trans  &trans  &trans    &trans  &trans  &trans  &trans   &kp F20  &kp F7
                             &trans  &trans  &trans    &trans  &trans  &trans
            >;
        };
        Config {
            display-name = "Config";
            bindings = <
        &bootloader  &trans  &trans  &trans  &to 4     &trans  &trans  &trans  &kp END  &kp F1
        &trans       &trans  &trans  &trans  &trans    &trans  &trans  &trans  &trans   &kp F10
&trans  &trans       &trans  &trans  &trans  &trans    &trans  &trans  &trans  &trans   &kp F20  &kp F7
                             &trans  &trans  &trans    &trans  &trans  &trans
            >;
        };
    };
};
