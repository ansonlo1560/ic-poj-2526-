# ic-poj-2526-
a ball rocbot which can move,play mp3 ,cry detech and more
MAX9814 + I2C MP3 + L9110S
1. 硬體接線 (MAX9814)
VCC -> Arduino 3.3V (MAX9814 接 3.3V 雜訊較少，比 5V 穩定)
GND -> Arduino GND
OUT -> Arduino A0 (原本 LM393 的 D2 拔掉，改接類比腳位 A0)
GAIN (如有) -> 懸空 (預設 60dB) 或接 VCC (40dB) 或接 GND (50dB)
2.這個版本加入了峰值檢測 (Peak-to-Peak)，能精確捕捉聲音震盪
實時監控：開啟序列埠監控器（或手機藍牙終端），你會看到 Volume: XXX
