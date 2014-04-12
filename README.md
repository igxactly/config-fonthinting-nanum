config-fonthinting-nanum
========================

우분투에서 발생하는 나눔글꼴 힌팅 문제를 해결하기 위한 글꼴 설정입니다. (우분투 14.04 KDE 환경에서 확인)
configuration for fixing font hinting issue of nanum fonts family on ubuntu (tested on ubuntu 14.04 with kde)

간단하게 이 설정을 적용하려면 터미널에서 다음 명령들을 실행하시고 로그아웃했다 다시 로그인하시면 됩니다.
To apply this configuration, simply paste-and-run these commands in your terminal. After running them you should re-login to desktop environment to see the result


빈 줄로 구분된 3개의 명령어임 these are three commands separated by blank lines


mkdir -p $HOME/.config/fontconfig/conf.d/

cd $HOME/.config/fontconfig/conf.d/

wget https://raw.githubusercontent.com/igxactly/config-fonthinting-nanum/master/90-fonts-nanum.conf





# 추후 더 좋은 설정값이 생긴다면 pull request 해주시거나 comment를 달아 알려주세요.
