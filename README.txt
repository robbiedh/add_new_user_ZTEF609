
telnet -> ip Router 

default password 
username : root	
password Zte521


For adding  new user 

sendcmd 1 DB p  DevAuthInfo
#menampilkan semua isi
sendcmd 1 DB set DevAuthInfo 5 Enable 1
# 5 -> row , Enable ->1 -> true
sendcmd 1 DB set DevAuthInfo 5 User root
#User -> username will be set
sendcmd 1 DB set DevAuthInfo 5 Pass toor123
# Pass -> set password for username
sendcmd 1 DB set DevAuthInfo 5 Level 0
# Level -> 0-> rooot, 1->admin
sendcmd 1 DB set DevAuthInfo 5 AppID 1
# AppID -> default 1
sendcmd 1 DB saveasy
# saving configure 