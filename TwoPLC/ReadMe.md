
Check the assoiation between the inspections and files.

files = bg~B194:0 bng~B195:0
bot ins = Top(1), Thread(2)
top ins = Thread(5), Catodioptric(6), Side(7), Top(8)

Bot		ins1 & ins2 g = B194:0  ng = B195:0
Top		load / align / set g = B194:0  ng = B195:0
		ins5 & ins7 g = B194:0  ng = B195:0
		ins6 & ins8 g = B194:0  ng = B195:0

boptic		= B194:0/[N7:1]
ins1		time data = get L28:[N7:13]  set L28:[N7:11]
			position data =  get L29:[N7:13]  set L29:[N7:11]
			pp = B194:0/[N15:5]
			g = B194:0/[N7:22]
			ng = B195:0/[N7:22]
ins2		time data = get L30:[N7:44]  set L30:[N7:43]
			position data =  get L31:[N7:44]  set L31:[N7:43]
			pp = B194:0/[N7:38]
			g = B194:0/[N7:41]
			ng = B195:0/[N7:41]
btransfer	g = B194:0/[N15:7]
			ng = B195:0/[N15:7]
Top Load	g = B194:0/[N15:6]
			ng = B195:0/[N15:6]
Top Optic	= B194:0/[N15:8]
			load I5 / I7 = B17:0/[N7:2]
			load I6 / I8 = B18
ins1		time data = get Lx:[x]  set Lx:[x]
			position data =  get Lx:[x]  set Lx:[x]
			pp = Bx:0/[x]
			g = Bx:0/[x]
			ng = Bx:0/[x]
ins2		time data = get Lx:[x]  set Lx:[x]
			position data =  get Lx:[x]  set Lx:[x]
			pp = Bx:0/[x]
			g = Bx:0/[x]
			ng = Bx:0/[x]




