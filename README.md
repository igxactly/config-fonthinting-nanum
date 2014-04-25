***freetype 버그로 보고 및 수정됨. 차후 우분투 저장소 패키지가 이 버그 수정에 대해서 업데이트되면 이 설정을 하실 필요가 없습니다. [https://savannah.nongnu.org/bugs/index.php?42148]***
2014. 4. 26. 기준 아직 업데이트 안 되었음.

config-fonthinting-nanum
========================

* 적용: 나눔고딕, 나눔명조, 나눔바른고딕, 나눔 손글씨 펜, 나눔 손글씨 붓

우분투에서 발생하는 나눔글꼴 힌팅 문제를 해결하기 위한 글꼴 설정입니다. (우분투 14.04 KDE 환경에서 확인)
configuration for fixing font hinting issue of nanum fonts family on ubuntu (tested on ubuntu 14.04 with kde)

간단하게 이 설정을 적용하려면 터미널에서 다음 명령들을 실행하시고 로그아웃했다 다시 로그인하시면 됩니다.
To apply this configuration, simply paste-and-run these commands in your terminal. After running them you should re-login to desktop environment to see the result


빈 줄로 구분된 3개의 명령어임 these are three commands separated by blank lines

`mkdir -p $HOME/.config/fontconfig/conf.d/`

`cd $HOME/.config/fontconfig/conf.d/`

`wget https://raw.githubusercontent.com/igxactly/config-fonthinting-nanum/master/90-fonts-nanum.conf`





-------------------------

* 참고로 이 설정은 시스템 전체에 적용되는 것이 아니라 로그인된 사용자에게만 적용됩니다.
In addition, this configuration method only affect locally on logined user, not system-wide.

* 추후 더 좋은 설정값이 생긴다면 pull request 해주시거나 comment를 달아 알려주세요.
Please notify me by a pull request or a comment, when you have got some better configuration.
