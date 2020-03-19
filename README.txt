in %appdata%\roaldcoin\ create a file named roaldcoin.conf with this code here
rpcuser=rpc_roaldcoin
rpcpassword=2fb758772c754d17d6b46769d
rpcallowip=127.0.0.1
rpcport=17205
listen=1
server=1

then (remove the mine.bat file already in the folder) in the file where you extraced the wallet create a file called mine.bat with this code here
@echo off
set SCRIPT_PATH=%cd%
cd %SCRIPT_PATH%
echo Press [CTRL+C] to stop mining.
:begin
 roaldcoin-cli.exe generate 1
goto begin

Enjoy:)