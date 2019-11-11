
files = bg-B194:0 bng-B195:0 tt-B194:0 tng-B195:0 tc1-B17:0 tc2-B18:0  
--top bad file is only 2048 but the top good files extend to 2560  
bot ins = Top(1), Thread(2)  
top ins = Thread(5), Catodioptric(6), Side(7), Top(8)  

  |  Function Zone  |  Data  |  
  |  ------------  |  -------------------------------------------  |  
  |    |    |  
  |  Bot  |  ins1 & ins2 g = B194:0  ng = B195:0    |  
  |  Top  |  load / align / set g = B194:0  ng = B195:0    |  
  |    |  ins5 & ins7 g = B194:0  ng = B195:0    |  
  |    |  ins6 & ins8 g = B194:0  ng = B195:0    |  
  |    |    |  
  |  boptic  |  = B194:0/[N7:1]    |  
  |  ins1  |  time data = get L28:[N7:13]  set L28:[N7:11]    |  
  |    |  position data =  get L29:[N7:13]  set L29:[N7:11]    |  
  |    |  pp = B194:0/[N15:5]-(105)    |  
  |    |  g = B194:0/[N7:22]    |  
  |    |  ng = B195:0/[N7:22]    |  
  |  ins2  |  time data = get L30:[N7:44]  set L30:[N7:43]    |  
  |    |  position data =  get L31:[N7:44]  set L31:[N7:43]    |  
  |    |  pp = B194:0/[N7:38]-(777)    |  
  |    |  g = B194:0/[N7:41]    |  
  |    |  ng = B195:0/[N7:41]    |  
  |  btransfer  |  g = B194:0/[N15:7]-(1356)    |  
  |    |  ng = B195:0/[N15:7]    |  
  |  Top Load  |  g = B194:0/[N15:6]-(100)    |  
  |    |  ng = B195:0/[N15:6]    |  
  |  Top Optic  |  = B194:0/[N15:8]-(1150)    |  
  |    |  load I5 / I7 = B17:0/[N7:2]    |  
  |    |  load I6 / I8 = B18:0/[N7:2]    |  
  |  ins5  |  time data = get L19:[N7:26]  set L19:[N7:25]    |  
  |    |  position data =  get L20:[N7:26]  set L20:[N7:25]    |  
  |    |  pp = B17:0/[N15:4]-(1502)    |  
  |    |  g = B17:0/[N7:27]    |  
  |    |  ng = B195:0/[N7:27]    |  
  |  ins6  |  time data = get L21:[N7:13]  set L21:[N7:10]    |  
  |    |  position data =  get L22:[N7:13]  set L22:[N7:10]    |  
  |    |  pp = B18:0/[N15:3]-(1512)    |  
  |    |  g = B18:0/[N7:14]    |  
  |    |  ng = B195:0/[N7:14]    |  
  |  ins7  |  time data = get L23:[N7:52]  set L23:[N7:58]    |  
  |    |  position data =  get L24:[N7:52]  set L24:[N7:58]    |  
  |    |  pp = B17:0/[N7:49]-(1515)    |  
  |    |  g = B17:0/[N7:56]    |  
  |    |  ng = B195:0/[N7:56]    |  
  |  ins8  |  time data = get L25:[N7:53]  set L25:[N7:59]    |  
  |    |  position data =  get L26:[N7:53]  set L26:[N7:59]    |  
  |    |  pp = B18:0/[N7:50]-(1520)    |  
  |    |  g = B18:0/[N7:57]    |  
  |    |  ng = B195:0/[N7:57]    |  
  |  Blow  |  B17:[N15:2] & B18:[N15:2]-(1976)    |  
  |    |    |  
  |  Slow Tests  |    |  
  |  Inspection 1 Trigger  |  N15:5 > 0 + (30 fixed?) (max part width)?    |  
  |    |  N15:5 < N7:38    |  
  |  Inspection 2 Trigger  |  N7:38 > N15:5    |  
  |    |  N7:38 < N15:7    |  
  |  bot transfer location  |  N15:7 > N7:38    |  
  |    |  N15:7 < 1399? (end of bs)    |  
  |  top load location  |  N15:6 > 70?    |  
  |    |  N15:6 < 130?    |  
  |  top optic location  |  N15:8 > 1000?    |  
  |    |  N15:8 < 1300?    |  
  |  Inspection 5 Trigger  |  N15:4 > N15:6 + (30 fixed?) (max part width)?    |  
  |    |  N15:4 < N15:3    |  
  |  Inspection 6 Trigger  |  N15:3 > N15:4    |  
  |    |  N15:3 < N7:49    |  
  |  Inspection 7 Trigger   |  N7:49 > N15:3    |  
  |    |  N7:49 < N7:50    |  
  |  Inspection 8 Trigger  |  N7:50 > N7:49    |  
  |    |  N7:50 < N15:2    |  
  |  Blow location  |  N15:2 > N7:50    |  
  |    |  N15:2 < (N7:11*16)+1440 Or (bs word offset*16)+(bs length) Or 2560    |  
  |    |    |  
  |  Fast Tests  |    |  
  |  Bot Optic Location  |  *N7:1 > 0    |  
  |    |  N7:1 < N15:5    |  
  |  Inspection 1 Result  |  *N7:22 > N15:5    |  
  |    |  N7:22 < N7:38    |  
  |  Inspection 2 Result  |  *N7:41 > N7:38    |  
  |    |  N7:41 < N15:7    |  
  |  top optic restult location  |  *N7:2 > N15:8 (1120)    |  
  |    |  N7:2 < N15:4    |  
  |  Inspection 5 Result  |  *N7:27 > N15:4    |  
  |    |  N7:27 < N7:49    |  
  |  Inspection 6 Result  |  *N7:14 > N15:3    |  
  |    |  N7:14 < N7:50    |  
  |  Inspection 7 Result  |  *N7:56 > N7:49    |  
  |    |  N7:56 < N15:2    |  
  |  Inspection 8 Result  |  *N7:57 > N7:50    |  
  |    |  N7:57 < N15:2    |  
  |    |    |  