# TIL
초간단 TIL 기록장

12/27 (월)
인스타그램 클론코딩, 프론트부분을 얼추 완성해보았다
처음해 보는 반응형 적용이라 여러모로 힘든점들이 많았지만 시간을 투자하니 얼추 그럴싸는 해진듯하다
웹개발강의 들으면서는 항상 px만 써왔어서 vw,vh, em,rem,%와 같은 단위가 어떤 의미를 가지는지 , 어떤경우에 써야되는지 전혀몰랐었으나
튜터님께서 제공해주신 example들을 보면서 조금이나마 더 깊게 알 수 있었고, display:flex 의 사용법도 몇가지 더 익혀볼 수 있었다 (언젠간 grid를 꼭 이해해보고싶다...)
미디어쿼리도 처음써보면서 되게 생소하고 신기하게 느껴졌는데, 사용자 편의에 있어 제일 필요한게 아닐까 싶었다
얼핏 짐작만 했을때와 달리 직접 작업을 해보니까 개발자들이 인류를 위해서 정말 많은 일들을 대신 귀찮아 주고 있는구나 싶은 하루였다
앞으로 이게 내 일이 될것이라 생각하니 참 설렌다 ㅋㅋㅋㅋㅋㅋㅋ 내가 다 대신 귀찮아주마!! 화...화이팅...


12/28 (화)
조가 바뀌고 기존에 만든 인스타 템플릿들을 통해 조원들과 함께 회원가입/로그인(jwt사용) + flask와 mongoDB를 활용해 본격적인 서비스 작업을 해보라는 미션을 받았다
솔직히 아직 뭐가뭔지 거의 잘 모르겠지만 그래도 flask와 DB를 활용해서 회원정보를 저장하고 해당 정보를 조회해 메인페이지로 이동하는 부분까진 어떻게든 해냈다
다만 jwt를 써서 같은 과정을 실행해 보니 암호화한 password를 저장하는 것 까지는 잘 되는데(DB에서 확인) 이걸 조회할때 뭔가 인식을 못하는 것 같다
구조를 얼추 이해하긴했는데 아직 미흡한 부분이 많나보다.......ㅠㅠ 내일 저녁까지 꼭 로그인부분을 완성해서 팀원들이 맡기로한 상세 페이지들 작업을 도와줄 수 있으면 좋겠다


12/29 (수)
여러 사람들의 도움과 구글신의 가호로 기적적으로 jwt를 이용한 로그인 구현에 성공했다
처음엔 구조도 뭔가 엄청 복잡하게 느껴지고 그랬는데 이제는 payload, secret_key , algorithm 으로 복합 encoding된 이친구가 어떤식으로 정보를 담고 돌아다니는지
그리고 인증정보가 필요한 각 페이지 들에서 이 토큰을 어떻게 사용해야 되는지 기본적인 부분은 이해할 수 있게 되었다
당장 다음주 화요일까지 프로젝트 완성해서 제출해야되는데 ... 조졌다.. 앞으로 거의 매일 밤을 새야되지 않을까 싶다......ㅠ



1/1 (토)
로그인 구현 이후에 각 페이지를 들어가면서 사용자 정보를 인증하기위한 유효성 검사를 삽입하였다. 그리고 main페이지에서 피드 추가 버튼을 눌렀을때
모달창을 띄우고 거기에 드롭된 이미지와 설명부분의 데이터를 받아와 db에 저장시키고 (이미지는 서버 단 media폴더에 저장 후 경로만 db에 저장)
피드 테이블에 저장된 모든 피드들을 자동으로 생성하는 것 까지 구현했다. 
개인사때문에 정신없던 것도있고 작업을 이해하면서 진행하느라 시간이 좀 오래걸리긴했는데, 터미널을 통해서 깃허브에 커밋했던 내용들이 왜인지 contribution에 적용이안됐더라...
매일 커밋을 올렸는데 이틀가량 초록색이어야할 내 잔디가 없어진게 너무 슬프다..ㅜㅜ


1/6 (목) - (과제 마감과 회복시간떄문에 몰아쓰는 오랜만의 TIL...)
인스타 클론코딩을 드디어(?) 얼추 완성했다.. 마감날까지 정신없이 코딩에만 집중했지만 처음부터 페이스를 그리 빨리 당긴편이 아니어서 발표때까지 썩 만족스러운
결과를 만들지 못했다... ㅠㅠ 잠깐의 휴식 후 고생한 팀원들과의 작품이 그지같은 상태로 올라가있는게 영 마음이 찝찝해서 혼자 보수작업에 착수
여전히 몇가지 문제점들은 남아있지만 그래도 어느정도는 그럴싸한 상태가 된 것 같다. 혼자서 해결하기 힘든문제들이 엄청나게 많았는데 그때마다 도와준 튜터님과 다른
친구들에게 감사한 마음도 들면서 한편으로는 서비스 하나 완성하는게 얼마나 어려운 일인지 깨닫게 된 좋은 경험이 되었다.
욕심만 많아가지고 이기능 저기능 넣어보자 하고 하나씩 작업해봤더니.. 하나 넣을떄마다 우후죽순처럼 생기는 문제점들에 정신을 못차리겠더라 ㅡㅜ
제일 기억에 남는 문제는 피드를 올렸을때 그 피드에 달린 좋아요나 북마크 버튼을 누르면, jinja로 뿌려줬던 데이터들을 가지고 어떻게 버튼을 누른 피드를 '특정'할 수 있냐는 것이었다
처음에는 피드 업로드 시에 임의로 주었던 인덱스 번호를 서버가 이해하는 과정에서 (test를위해) db 삭제/수정시 중간중간 중복되는 경우가 발생해서 문제가 생기는 것인가? 라고
생각해서 피드 참조 인자를 db에서 데이터 입력시에 자동 생성해주는 id 값으로 변경도 해보았다. 그러나 여전히 좋아요나 북마크, 댓글버튼을 누르면 제일 최상단에 있는 피드에
기능이 작동하는것을보고 살짝 멘붕이 왔다가, 처음부터 jinja 반복문으로 피드데이터를 뿌려줄때 좋아요, 댓글, 북마크 같이 타겟 지정이 필요한 버튼들에 피드 id를 온클릭 파라미터로
담아버리면 되는구나! 라는 사실을 알고 유레카를 외쳤던 기억이 가장 머리에 남는다
이 외에도 db컬렉션, api 설계등등을 작업 초반에 제대로 하지못해서(사실 시작할땐 이게 이렇게 중요한줄도, 어떻게 해야되는지도 모름..) 피드를 업로드 해놓은 이후 내 프로필 설정을
바꾸면 기존에 올려놨던 피드들에 담겨있던 작성자 프로필사진/닉네임 과 같은 데이터들이 같이 바뀌지 않아서 세상이 무너졌던 기억도 있고
마이페이지를 꾸미면서 구성해논 북마크들을 모아놓은 부분이 mypage.html 에서 버튼을 누르면 자바스크립트를 통해 동작하게 해놨었는데.. 메인페이지에서 바로 이 북마크 모음 부분으로
바로 이어주는 버튼을 만들려고 하니 (똑같은 페이지를 하나 더 만들어서 해결하는 건 뭔가 이상하다는 생각이...) 이 또한 쉽게 해결이 되지않아 특정 북마크 버튼을 누르면 status값을
같이 서버로 전송하고, 다시 마이페이지에 리턴해온 status 값에 따라 $(document).ready(function()) 이 별도로 작동하게 만들었더니 어찌저찌 또 원하는바를 달성하게 되었다 ㅋㅋㅋ
일주일 가량의 시간동안 정말 다 적지못할만큼 수많은 에러에 부딪치고 해결하고, 다음문제를 해결하려 뭔가를 바꿧더니 다시 이전 문제가 발생하는 이런 거지같은 상황을 매일 경험하다보니
코딩 실력도 실력이지만 멘탈이 정말 튼튼해져가는 기분이 들었다. 이제는 에러메시지를 봐도 당황은 커녕.. 음.. 또 만났군 녀석.. 을 시전하며 태연하게 에러난 위치를 찾아나가게된
내 모습을 보며 알수없는 뿌듯함이 느껴진 프로젝트였다 이제 자야지..


1/20 (목)
한동안 몰입해있던 머신러닝 프로젝트를 뒤로하고 장고 수업이 시작되었다 아직까지는 기본 구성에 대한 이해라 크게 어려운건 없는것 같다
수업을 이미 거의 다들은 친구가 말하기론 플라스크 쓸때보다 훨~씬 더 쉽고 편하다고 해서 매우 기대가 된다 ㅎㅎㅎ
아참 TIL을 너무 오랜기간동안 쉬었는데, 곰곰히 고민을 해보니까 처음의 취지와는 다르게 너무 복잡하고 열심히 쓰려고 했던게 부담이 된 것 같다
물론 다 변명이지만 프로젝트기간동안 너무 지치고 힘들어서 그런것도 있... 크흠..
앞으로 더 짧고 간결하게 느낀점만 쓰고 끝내야겠다 !! 다시 꾸준해질수 있기를... 화이팅!


1/24 (월)
알고리즘 스터디에서 오늘 풀기로 했던 문제중 하나가 너무 어려워서 하루죙일 해맸다... 탐욕법을 활용한 문제였는데 아직도 답을 찾지 못했다 ㅠㅠ
다른문제들은 다 풀었는데 저거 하나 못풀었다고 하루가 내내 찝찝한 느낌,, 일단 곧 시작하게될 장고 프로젝트를 준비하기 위해서
아쉬움을 뒤로하고 나중을 기약하기로 했다. 내일은 좀더 뿌듯한 하루가 될 수 있게 컨디션 조절부터 열심히 해야지..


1/26 (수)
장고와 머신러닝을 활용한 새로운 프로젝트가 시작되었다. 선형회귀에서의 cosine similarity를 통한 일치율을 계산하여 연관성있는 정보를 찾아주는 것이 주된 포인트다
넷플릭스를 기준으로는, 사용자의 기호와 관련된 입력값을 받아 취향에 맞는 작품들을 상단에 노출시켜주는 형태도 이와 같다 볼수있다
우리조는 사용자의 선호 플레이스타일을 입력받아 취향에 맞을법한 롤 챔피언을 추천하는 서비스를 만들어 보려고한다
구상은 참 야무졌는데 얼마나 실현가능하게 될지는 두고봐야할것같다 ㅎㅎㅎ 최선을 다해보자..!


1/27 (목)
이번에는 프론트엔드를 맡아서 화면 구성을 열심히 해보았다. 처음으로 html에 동영상을 넣어봤는데 크롬/파이어폭스에서는 정책상 autoplay가 원활히 안되는 경우가 많아서
video태그에 muted 를 넣어줘야지만 자동재생이 가능한 상황이 연출됐다, 그래서 별도의 css와 자바스크립트를 통해 mute / unmute 버튼을 달아주는것으로 해결했다
뭔가 html / css 하면 굉장히 기본적이고 쉬운 것 이란 생각을 잠시 했었는데 이 또한 엄청난 오만이었던것 같다... 파면 팔수록 더 공부해야될게 나오니 ㅎㅎ...
내일까지 프론트를 개략적이나마 다 마치고 얼른 백엔드/머신러닝 팀을 도와주러 가야겠다 ㅎㅅㅎ


2/16 (수)
프로젝트에 치이다가 번아웃와서 거진 3주만에 쓰는 TIL...
연휴고 뭐고 밤낮없이 작업해서 발표회때 좋은 반응을 얻기는 했지만 막상 시스템 구성상 꼭 들어가야하는 일부 크롤링 코드들이
본 페이지 업데이트로 인해 div구조가 전반적으로 바뀌면서 먹통이되었다...damn..
조만간 요거 고쳐서 내 repo에 다시 올려봐야겠당


2/17 (목)
넘쳐나는 강의에 압도될것만 같다.. ㅋㅋㅋ 일단 다음 프로젝트에 직결되는 부분인 open cv 관련파트를 먼저 공부하게 됐다
각종 이미지와 동영상과같은 컨텐츠들을 다른 모델들과 함께 전/후처리를 통하여 합성(?) 하는 방법과 더불어 다양하게 수정해보는 것을 연습해보았다
숙제 제출을 위해서 하나의 이미지를 4가지의 다른 모델들로 blob시켜 조합해봤는데 쉽지않았다
단순히 x축 axis만 가지고 4등분하여 이어붙이는건 간단했지만 뭔가 예술적이지 못한 느낌이 들어 비대칭형식으로 시도한게 원인인것 같았다
그래서 약간의 노가다를 섞어, 원하는 파트 4곳의 cropping point를 따로 설정하고 각각 변수에 담아 합성시킨뒤 기존 원본 img팔레트 위에 덧입히는 식으로 하니
왜 돼는건지는 잘 모르겠지만 일단 결과물을 얻을 수 있었다..!

<원본>
![image](https://user-images.githubusercontent.com/92630511/154506802-10256130-7256-450b-b43f-a2859bca47c0.png)


<변경후>
![image](https://user-images.githubusercontent.com/92630511/154506581-44a9f859-c1e9-496b-84e8-3c5b554fa569.png)

요즘 약간 번아웃오는것같이 힘들고 집중도안오고 그랬는데, 뭔가 재밌는 작업을하니 다시 의지가 샘솟는 기분이들어 매우 만족스런 하루였다ㅎㅎㅎ 내일도 화이팅!



