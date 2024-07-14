import random


data = [
    {
        'name': "Virat kohli",
        'Team': "India",
        'followers': 256
    }
    ,

    {
        'name': "Ms dhoni",
        'Team': "India",
        'followers': 44
    }
    ,

    {
        'name': "Subhmangill",
        'Team': "India",
        'followers': 54
    }
    ,
    {
        'name': "Sachin tendulkar",
        'Team': "India",
        'followers': 87
    }
    , {
        'name': "Yashasvi jaiswal",
        'Team': "India",
        'followers': 34
    }
    ,
    {
        'name': "Jaspreet bumrah",
        'Team': "India",
        'followers': 80
    },
    {
        'name': "Arshdeep singh",
        'Team': "India",
        'followers': 39
    }, {
        'name': "Hardik pandya",
        'Team': "India",
        'followers': 32
    },
    {
        'name': "Rohit sharma",
        'Team': "India",
        'followers': 102
    }
    , {
        'name': "Rishabh pant",
        'Team': "India",
        'followers': 59
    }
]

current_score = 0
def choose_player():
    print("""                                                                       
        ,--,                               ,--,                        
      ,--.'|    ,---,   ,----..          ,--.'|     ,---,. ,-.----.    
   ,--,  | : ,`--.' |  /   /   \      ,--,  | :   ,'  .' | \    /  \   
,---.'|  : ' |   :  : |   :     :  ,---.'|  : ' ,---.'   | ;   :    \  
|   | : _' | :   |  ' .   |  ;. /  |   | : _' | |   |   .' |   | .\ :  
:   : |.'  | |   :  | .   ; /--`   :   : |.'  | :   :  |-, .   : |: |  
|   ' '  ; : '   '  ; ;   | ;  __  |   ' '  ; : :   |  ;/| |   |  \ :  
'   |  .'. | |   |  | |   : |.' .' '   |  .'. | |   :   .' |   : .  /  
|   | :  | ' '   :  ; .   | '_.' : |   | :  | ' |   |  |-, ;   | |  \  
'   : |  : ; |   |  ' '   ; : \  | '   : |  : ; '   :  ;/| |   | ;\  \ 
|   | '  ,/  '   :  | '   | '/  .' |   | '  ,/  |   |    \ :   ' | \.' 
;   : ;--'   ;   |.'  |   :    /   ;   : ;--'   |   :   .' :   : :-'   
|   ,/       '---'     \   \ .'    |   ,/       |   | ,'   |   |.'     
'---'                   `---`      '---'        `----'     `---'       
                                                                       
                   ,--,                                                           
                ,---.'|        ,----..                                            
                |   | :       /   /   \              .---.     ,---,. ,-.----.    
                :   : |      /   .     :            /. ./|   ,'  .' | \    /  \   
                |   ' :     .   /   ;.  \       .--'.  ' ; ,---.'   | ;   :    \  
                ;   ; '    .   ;   /  ` ;      /__./ \ : | |   |   .' |   | .\ :  
                '   | |__  ;   |  ; \ ; |  .--'.  '   \' . :   :  |-, .   : |: |  
                |   | :.'| |   :  | ; | ' /___/ \ |    ' ' :   |  ;/| |   |  \ :  
                '   :    ; .   |  ' ' ' : ;   \  \;      : |   :   .' |   : .  /  
                |   |  ./  '   ;  \; /  |  \   ;  `      | |   |  |-, ;   | |  \  
                ;   : ;     \   \  ',  /    .   \    .\  ; '   :  ;/| |   | ;\  \ 
                |   ,/       ;   :    /      \   \   ' \ | |   |    \ :   ' | \.' 
                '---'         \   \ .'        :   '  |--"  |   :   .' :   : :-'   
                               `---`           \   \ ;     |   | ,'   |   |.'     
                                                '---"      `----'     `---'       
                                                                            """)
    global player1,player2
    player1 = []

    player2 = []


    order1 = random.randint(0, 9)
    player1.append(data[order1])
    # print(player1)

    a=data.pop(order1)


    # print(data)
    b=len(data)
    order2 = random.randint(0,b-1 )
    # print(order2)

    player2.append(data[order2])
    print(f"Current score:{current_score}")
    print(f"Compare A: {player1[0]['name']},{player1[0]['Team']}")

    print("""            
       ,---. 
      /__./| 
 ,---.;  ; | 
/___/ \  | | 
\   ;  \ ' | 
 \   \  \: | 
  ;   \  ' . 
   \   \   ' 
    \   `  ; 
     :   \ | 
      '---"  
                                                                                    
                                                                                                           
    .--.--.    
   /  /    '.  
  |  :  /`. /  
  ;  |  |--`   
  |  :  ;_     
   \  \    `.  
    `----.   \ 
    __ \  \  | 
   /  /`--'  / 
  '--'.     /  
    `--'---'   
            """)
    print(f"Against B: {player2[0]['name']},{player2[0]['Team']}")
    data.append(a)

    # print(player2)
choose_player()
A = player1[len(player1)-1]['followers']
B = player2[len(player2)-1]['followers']

def compare(A,B):

    global current_score

    choose = input("Who has more followers? Type 'A' or 'B' : ")
    if (choose == 'A'):
        if (A > B):
            print(f" A has {A} follower And you Choose correct ")
            current_score+=1
            print(f"Current score:{current_score}")
            choose_player()
            compare(A,B)
            return


        else:
            print("You choose wrong")
            print(f"Current score:{current_score}")

            return
    elif(choose=='B'):
        if (B>A):
            print(f" B has {B} follower And you Choose correct ")

            current_score+=1


            choose_player()
            compare(A,B)

            return current_score
        else:
            print("You choose wrong")
            print(f"Current score:{current_score}")
            return

compare(A,B)




