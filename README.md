# znaaz-chatbot

import re

pattern ="[a-zA-Z]"


while True:
    print("chatbot:","hi I'm eliza,may I know your name?")
    request=input("user:")
    
    
  
    if(request.lower()=="bye"):
        print("chatbot:bye")
        break    
    else:
        request_name0=re.sub("hi,i am"," ",request.lower())
        request_name=re.sub('i am'," ",request.lower())
        request_name2=re.sub("my name is"," ",request.lower())
        request_name3=re.sub("this is"," ",request.lower())
        request_name4=re.sub("here"," ",request.lower())
        
        relationship="brother mother father sister friend mom mummy papa pappa dad boy "
        
        
        feel="good great upset bad happy ok happi sad grief fine not joy afraid fear fright anger depress content surprise disgust angry cheer"
      
        verb=[]
        verb='end','start','do', 'want', 'need', 'look'
       
        ngood="feeling good"
       
        nhappy="feeling happy"
        nfine="not fine"
        
        fear=re.findall("fear",feel)
        happi=re.findall("happi",feel)
        nott=re.findall("not",feel)
        good=re.findall("good",feel)
        bad=re.findall("bad",feel)
        happy=re.findall("happy",feel)
        sad=re.findall("sad",feel)
        fine=re.findall("fine",feel)
        cheer=re.findall("cheer",feel)
        grief=re.findall("grief",feel)
        joy=re.findall("joy",feel)
        afraid=re.findall("afraid",feel)
        fright=re.findall("fright",feel)
        anger=re.findall("anger",feel)
        ok=re.findall("ok",feel)
        depress=re.findall("depress",feel)
        content=re.findall("content",feel)
        surprise=re.findall("surprise",feel)
        disgust=re.findall("disgust",feel)
        angry=re.findall("angry",feel)
        cheer=re.findall("cheer",feel)
        mother=re.findall("mother",relationship)
        father=re.findall("father",relationship)
        brother=re.findall("brother",relationship)
        sister=re.findall("sister",relationship)
        friend=re.findall("friend",relationship)
        boy=re.findall("boy",relationship)
        mom=re.findall("mom",relationship)
        mummy=re.findall("mummy",relationship)
        mommy=re.findall("mommy",relationship)
        dad=re.findall("dad",relationship)
        daddy=re.findall("daddy",relationship)
        papa=re.findall("papa",relationship)
        pappa=re.findall("pappa",relationship)
        upset=re.findall("upset",feel)
        great=re.findall("great",feel)
        
        
        first0="hi,i am"+request_name0
        first_statement0=re.sub(" +"," ",first0)
        
        first ="i am"+request_name
        first_statement=re.sub(" +"," ",first)
        
        second="my name is"+request_name2
        second_statement=re.sub(" +"," ",second)
        third="this is"+request_name3
        third_statement=re.sub(" +"," ",third)
        
        fourth=request_name4+"here"
        fourth_statement=re.sub(" +"," ",fourth)
        
        display0="chatbot:hi"+request_name0+", how are you doing today?"
        actual_display0=re.sub(" +"," ",display0)
        display="chatbot:hi"+request_name+", how are you doing today?"
        
        actual_display=re.sub(" +"," ",display)
        display2="chatbot:hi"+request_name2+", how are you doing today?"
        actual_display2=re.sub(" +"," ",display2)
        display3="chatbot:hi"+request_name3+", how are you doing today?"
        actual_display3=re.sub(" +"," ",display3)
       
        display4="chatbot:hi "+request_name4+", how are you doing today?"
        actual_display4=re.sub(" +"," ",display4)
        display5="chatbot:hi "+request+", how are you doing today?"
        actual_display5=re.sub(" +"," ",display5)
        
        
        if (request.lower()==first_statement0): 
            print(actual_display0)
        elif(request.lower()==first_statement):
            print(actual_display)
        elif(request.lower()==second_statement):
            print(actual_display2)
        elif(request.lower()==third_statement):
           
            print(actual_display3)
        elif(request.lower()==fourth_statement):
            print(actual_display4)  
            
        else:
            print(actual_display5)
            
        request2=input("user:")
        if(request2.lower()=="bye"):
         print("chatbot:bye")
         break  
        else:
            if (re.findall("not",request2.lower())!=nott):
                if (re.findall("great",request2.lower())==great) :
                    print("chatbot:That's nice!how may I help you?")
                if (re.findall("good",request2.lower())==good):
                    print("chatbot:That's great!how may I help you?")
                if (re.findall("ok",request2.lower())==ok) :
                    print("chatbot:That's good!how may I help you?")
                elif(re.findall("fine",request2.lower())==fine):
                    print("chatbot:That's great!how may I help you?")
                elif(re.findall("bad",request2.lower())==bad):
                    print("chatbot:I'm sorry to hear that,how can I help you?")
                elif(re.findall("sad",request2.lower())==sad):
                    print("chatbot:I'm sorry to hear that,how can I help you?")
                elif(re.findall("happy",request2.lower())==happy):
                    print("chatbot:That's great!,how may I help you?") 
            elif(re.findall("not",request2.lower())==nott):
               
                if(re.findall("good",request2.lower())==good):
                    print("chatbot:I'm sorry to hear that,how can I help you?")
                elif(re.findall("ok",request2.lower())==ok):
                    print("chatbot:I'm sorry to hear that,how can I help you?")
                elif(re.findall("feeling good",request2.lower())==ngood):
                    print("chatbot:I'm sorry to hear that,how can I help you?")          
                elif(re.findall("happy",request2.lower())==happy):
                    print("chatbot:I'm sorry to hear that,how can I help you?")
                elif(re.findall("chatbot:feeling happy",request2.lower())==nhappy):
                    print("chatbot:I'm sorry to hear that,how can I help you?")
                elif(re.findall("fine",request2.lower())==fine):
                    print("chatbot:I'm sorry to hear that,how can I help you?")
                    
       
         
       
        request3=input("user:")
        if(request3.lower()=="bye"):
         print("chatbot:bye")
         break
        else:
            
            
            if(re.findall("happy",request3.lower())==happy):
                    print("chatbot:That's nice!")
                    request3=input("user:")
            if(re.findall("joy",request3.lower())==joy):
                    print("chatbot:That's nice!")
                    request3=input("user:")
            if(re.findall("happi",request3.lower())==happi):
                 print("chatbot:That's nice!")
                 request3=input("user:")
            if(re.findall("cheer",request3.lower())==cheer):
                 print("chatbot:That's nice!")
                 request3=input("user:")
            if(re.findall("surprise",request3.lower())==surprise):
                 print("chatbot:That's cool!")
                 request3=input("user:")
            if(re.findall("content",request3.lower())==content):
                 print("chatbot:That's nice!")
                 request3=input("user:")
            if(re.findall("sad",request3.lower())==sad):
                    print("chatbot:I'm sorry to hear that")
                    request3=input("user:")
            if(re.findall("upset",request3.lower())==upset):
                    print("chatbot:I'm sorry to hear that")
                    request3=input("user:")
            if(re.findall("disgust",request3.lower())==disgust):
                    print("chatbot:I'm sorry to hear that")
                    request3=input("user:")
            if(re.findall("grief",request3.lower())==grief):
                    print("chatbot:I'm sorry to hear that")
                    request3=input("user:")
            if(re.findall("angry",request3.lower())==angry):
                    print("chatbot:Yeah,I can understand.")
                    request3=input("user:")
            
            
            if(re.findall("fear",request3.lower())==fear):
                  print("chatbot:Oh, don't worry, that's fine.It's ok to have fears.")
                  request3=input("user:")
            if(re.findall("fright",request3.lower())==fright):
                 print("chatbot:I'm sorry to hear that,but don't worry, that's fine.")
                 request3=input("user:")
            if(re.findall("depress",request3.lower())==depress):
                 print("chatbot:I'm sorry to hear that")
                 request3=input("user:")
            if(re.findall("afraid",request3.lower())==afraid):
                 print("chatbot:I'm sorry to hear that,but don't worry, that's fine.")
                 request3=input("user:")
            if(re.findall("anger",request3.lower())==anger):
                 print("chatbot:Yeah,I can understand.")
                 request3=input("user:")
            
            
            
           
                          
            
            elif(re.findall("mother",request3.lower())==mother):
                 print("chatbot:what does your mother do?")
                 request4=input("user:")
                 if(re.findall(pattern,request4.lower())):
                     print("chatbot:I see..,tell me something more")
                     request3=input("user:")
                 
            elif(re.findall("father",request3.lower())==father):
                 print("chatbot:what does your father do?")
                 request4=input("user:")
                 if(re.findall(pattern,request4.lower())):
                     print("chatbot:I see..,tell me something more")
                     request3=input("user:")
           
            elif(re.findall("mom",request3.lower())==mom):
                 print("chatbot:what does your mom do?")
                 request4=input("user:")
                 if(re.findall(pattern,request4.lower())):
                     print("chatbot:I see..,tell me something more")
                     request3=input("user:")
            
            elif(re.findall("mummy",request3.lower())==mummy):
                 print("chatbot:what does your mummy do?")
                 request4=input("user:")
                 if(re.findall(pattern,request4.lower())):
                     print("chatbot:I see..,tell me something more")
                     request3=input("user:")
            
            elif(re.findall("papa",request3.lower())==papa):
                 print("chatbot:what does your papa do?")
                 request4=input("user:")
                 if(re.findall(pattern,request4.lower())):
                     print("chatbot:I see..,tell me something more")
                     request3=input("user:")
            
            elif(re.findall("pappa",request3.lower())==pappa):
                 print("chatbot:what does your pappa do?")
                 request4=input("user:")
                 if(re.findall(pattern,request4.lower())):
                     print("chatbot:I see..,tell me something more")
                     request3=input("user:")
            
            elif(re.findall("dad",request3.lower())==dad):
                 print("chatbot:what does your daddy do?")
                 request4=input("user:")
                 if(re.findall(pattern,request4.lower())):
                     print("chatbot:I see..,tell me something more")
                     request3=input("user:")
            
            elif(re.findall("brother",request3.lower())==brother):
                 print("chatbot:what does your brother do?")
                 request4=input("user:")
                 if(re.findall(pattern,request4.lower())):
                     print("chatbot:I see..,tell me soomething more")
                     request3=input("user:")
            
            elif(re.findall("sister",request3.lower())==sister):
                 print("chatbot:what does your sister do?")
                 request4=input("user:")
                 if(re.findall(pattern,request4.lower())):
                     print("chatbot:I see..,tell me something more")
                     request3=input("user:")
                 
            elif(re.findall("boy",request3.lower())==boy and re.findall("friend",request3.lower())==friend):
                 print("chatbot:what does your boy friend do?")
                 request4=input("user:")
                 if(re.findall(pattern,request4.lower())):
                     print("chatbot:I see..,tell me something more")
                     request3=input("user:")
                 
            elif(re.findall("friend",request3.lower())==friend and re.findall("boy",request3.lower())!=boy ):
                 print("chatbot:what does your friend do?")
                 request4=input("user:")
                 if(re.findall(pattern,request4.lower())):
                     print("chatbot:I see..,tell me something more")
                     request3=input("user:")
                 
                      
            verb=(re.findall(r'\b(\w+ed)\b',request3.lower()))
           
            verbstr=str(verb)
            verbstrdisplay=verbstr.lstrip("'[").rstrip("']")
            upverb=re.sub("ed","",verbstr,1)
            
            upverbdisplay=upverb.lstrip("['").rstrip("']")
            
            resp1="chatbot:oh did you ?"
            resp2="chatbot:why did it "+upverbdisplay+ " ?"
            resp3="chatbot:when did it "+upverbdisplay+" ?"
            
            if(len(verb)!=0):
              
               
                  if((request3.split()[0].lower()=="i" or "I" and len(request3.split()[0].lower())==1
                      ) or re.findall(verbstr,request3.lower())==request3.split()[0].lower()):
 
                       print(resp1)
                  
              
    
                  elif( (request3.split()[-1]==verbstrdisplay)):
                   print(resp3)
                   
                  else:
                   print(resp2)
                   
                  while True:
                       request3=input("user:")
                       
                       if(request3.lower()!="bye" ):
                           if(re.findall("mother",request3.lower())==mother):
                               print("chatbot:what does your mother do?")
                               request4=input("user:")
                               if(re.findall(pattern,request4.lower())):
                                   print("chatbot:I see..,tell me something more")
                                   #request3=input("user:")
                           
                           elif(re.findall("father",request3.lower())==father):
                               print("chatbot:what does your father do?")
                               request4=input("user:")
                               if(re.findall(pattern,request4.lower())):
                                   print("chatbot:I see..,tell me something more")
                                   #request3=input("user:")
           
                           elif(re.findall("mom",request3.lower())==mom):
                              print("chatbot:what does your mom do?")
                              request4=input("user:")
                              if(re.findall(pattern,request4.lower())):
                                  print("chatbot:I see..,tell me something more")
                                  #request3=input("user:")
            
                           elif(re.findall("mummy",request3.lower())==mummy):
                               print("chatbot:what does your mummy do?")
                               request4=input("user:")
                               if(re.findall(pattern,request4.lower())):
                                   print("chatbot:I see..,tell me something more")
                                   #request3=input("user:")
            
                           elif(re.findall("papa",request3.lower())==papa):
                               print("chatbot:what does your papa do?")
                               request4=input("user:")
                               if(re.findall(pattern,request4.lower())):
                                   print("chatbot:I see..,tell me something more")
                                   #request3=input("user:")
            
                           elif(re.findall("pappa",request3.lower())==pappa):
                               print("chatbot:what does your pappa do?")
                               request4=input("user:")
                               if(re.findall(pattern,request4.lower())):
                                   print("chatbot:I see..,tell me something more")
                                   #request3=input("user:")
            
                           elif(re.findall("dad",request3.lower())==dad):
                               print("chatbot:what does your daddy do?")
                               request4=input("user:")
                               if(re.findall(pattern,request4.lower())):
                                   print("chatbot:I see..,tell me something more")
                                   #request3=input("user:")
            
                           elif(re.findall("brother",request3.lower())==brother):
                               print("chatbot:what does your brother do?")
                               request4=input("user:")
                               if(re.findall(pattern,request4.lower())):
                                   print("chatbot:I see..,tell me soomething more")
                                   #request3=input("user:")
            
                           elif(re.findall("sister",request3.lower())==sister):
                               print("chatbot:what does your sister do?")
                               request4=input("user:")
                               if(re.findall(pattern,request4.lower())):
                                   print("chatbot:I see..,tell me something more")
                                   #request3=input("user:")
                 
                           elif(re.findall("boy",request3.lower())==boy and re.findall("friend",request3.lower())==friend):
                              print("chatbot:what does your boy friend do?")
                              request4=input("user:")
                              if(re.findall(pattern,request4.lower())):
                                  print("chatbot:I see..,tell me something more")
                                  #request3=input("user:")
                 
                           elif(re.findall("friend",request3.lower())==friend and re.findall("boy",request3.lower())!=boy ):
                              print("chatbot:what does your friend do?")
                              request4=input("user:")
                              if(re.findall(pattern,request4.lower())):
                                  print("chatbot:I see..,tell me something more")
                                  #request3=input("user:")
                 
                               
                       else:
                        print("chatbot:bye")
                        break          
                  break
            
                       
                       
                
                 
       
    
                      
                
            
            
            
           
            
            
            
           
           
