点融网
https://www.dianrong.com/images/captcha.jpg

---------------------------------------------------------------------------------------------
Captcha_URL="https://www.dianrong.com/images/captcha.jpg"
while true
do
	pic_file=`date "+%Y%m%d_%H%M%S.jpg"`
	#wget --no-check-certificate https://www.dianrong.com/images/captcha.jpg -O ${pic_file}
	curl -k -H "Host:www.dianrong.com"  ${Captcha_URL}  -o ${pic_file}
	sleep 3
done
---------------------------------------------------------------------------------------------