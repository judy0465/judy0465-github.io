---
marp: true
theme: uncover
class: invert
paginate: true
header: Marp tutorial
footer: 2023-02-10
---

<!--_color: pink-->
### <span style="color:gray;">Unity</span>
# Project_VR_shared_space

---

## Index <!--_color: pink-->
#### Scene 정리
- ABCD scenes table 




---
<!--_color: pink-->
# ABCD Scenes
---

File_name| Screenshoot | Scene_name
---------|:-------------------------------:|:-----
index | ![h:150](./project_vr/scene_index.jpg) | ■ 비트월드.
AScene | ![h:150](./project_vr/scene_a.jpg) | ■ 음극선관.
A2Scene | ![h:150](./project_vr/scene_a2.jpg) | 인트로.

---

File_name| Screenshoot | Scene_name
---------|:-------------------------------:|:-----
BScene   |![h:150](./project_vr/scene_b.jpg) | ■ LED.
B2Scene| ![h:150](./project_vr/scene_b2.jpg) | ■ 네트워크.
CScene | ![h:150](./project_vr/scene_c.jpg) | 가상.

---

File_name| Screenshoot | Scene_name
---------|:-------------------------------:|:-----
DScene | ![h:150](./project_vr/scene_d.jpg) | 프레임.
D2Scene | ![h:150](./project_vr/scene_d2.jpg) | ■ 가상 현실.
FScene | ![h:150](./project_vr/scene_f.jpg) | 로우 폴리곤.

---

File_name| Screenshoot | Scene_name
---------|:-------------------------------:|:-----
GScene | ![h:150](./project_vr/scene_g.jpg) | ■ 인터넷.
G2 | ![h:150](./project_vr/scene_g2.png) | ■ 트랜지스터.
grabscene | ![h:150](./project_vr/scene_grab.jpg) | 조립 테스트.

---

File_name| Screenshoot | Scene_name
---------|:-------------------------------:|:-----
Practice_Light| ![h:150](./project_vr/scene_practice_light.jpg) | 발사 테스트.  
spaecShip| ![h:150](./project_vr/scene_spaceship.jpg) | 우주선 에셋.
X_Space_Test | ![h:150](./project_vr/scene_x_space_test.jpg) | 공간 테스트.

---

# Build Settings
#####  경로: 위치: [파일]-'Build settings'

---

Scene number<br>
![](./unity_/build_settings.jpg)

---

project window | assets > script > sceneChanger.cs


---
<!--_color: pink-->

#####  Quad 를 사용하여 이미지 첨부하는 방법!

###### 1. 하이라키 창에서 우클릭- 3D Object - Quad 클릭

![bg right w:500](./project_vr/i_1_hierarchy.jpg)
구글 업로드 해서 사진 바꾸기!!

---

###### 2. Project 창에서 우클릭- Create - Material

![bg right w:500](./project_vr/i_2_project.jpg)

---

###### 3. 내가 만든 Material을 클릭- Inspector 창에서 윗 부분에 shader 칸에서 '**Universal Render Pipeline**' 클릭 

![bg right w:500](./project_vr/i_3_shade.jpg)

---
###### 4. Lit(기본설정) -> 'Unlit'으로 바꿔주기
- ###### Lit- 조명의 영향 O
- ###### Unlit- 조명의 영향X

![bg right w:500](./project_vr/i_3_2_unlit.jpg)

---

###### 5. Inspector 창의 밑 부분에 Surface Inputs-     Base Map에 원하는 이미지 드래그 해서 가져오기.(끝)

![bg right w:500](./project_vr/i_3_surfaceinputs.jpg)


---
<!--_color: pink-->
#####  UI 사용하여 이미지 첨부하기

1. 
![bg right w:500](./project_vr/ui_image.jpg)
![bg right w:500](./project_vr/ui_result.jpg)

---
2.

![bg w:500](./project_vr/add_asset.jpg)


---

3.

![bg  w:500](./project_vr/add_image.jpg)


---

4. 이미지 첨부 완료.

![bg right w:500](./project_vr/change_sprite.jpg)


---

#####  Quad 를 사용하여 이미지 첨부하는 방법!

###### 1. 하이라키 창에서 우클릭- 3D Object - Quad 클릭

![bg right w:500](./project_vr/i_1_hierarchy.jpg)
구글 업로드 해서 사진 바꾸기!!

---

###### 2. Project 창에서 우클릭- Create - Material

![bg right w:500](./project_vr/i_2_project.jpg)

---

###### 3. 내가 만든 Material을 클릭- Inspector 창에서 윗 부분에 shader 칸에서 '**Universal Render Pipeline**' 클릭 

![bg right w:500](./project_vr/i_3_shade.jpg)

---
###### 4. Lit(기본설정) -> 'Unlit'으로 바꿔주기
- ###### Lit- 조명의 영향 O
- ###### Unlit- 조명의 영향X

![bg right w:500](./project_vr/i_3_2_unlit.jpg)

---

###### 5. Inspector 창의 밑 부분에 Surface Inputs-     Base Map에 원하는 이미지 드래그 해서 가져오기.(끝)

![bg right w:500](./project_vr/i_3_surfaceinputs.jpg)


---



### Unity Errors 모음
<!--_color: yellow-->
Case 1)

![h:100](./image/errors_1.jpg) 
-해결방법: Project-Oculus-VR-Plugins 에서 1.74.0만 남겨두고 나머지 삭제.

---

- ##### 해결 후 화면: 
![h:300](./image/errors_1_solution.jpg) 
: plugin 안에 2개의 파일만 존재한다.

---

<!--_color: yellow-->

case 2)
- 프로젝트 동기화가 되지 않을 때

![width:500](./project_vr/e1.jpg)

######  1. 유니티 허브 상에서 맨 밑의 주소를 확인한 다음,저장되어 있는 주소로 찾아가서 프로젝트 폴더를 지운다.


---
<!--_color: yellow-->
###### 2. 유니티 허브에서 open 버튼을 눌러 Open remote project를 누른다.

![width:500](./project_vr/e1.jpg)



---
<!--_color: yellow-->
![width:500](./project_vr/e2.jpg)

###### 3. 해당 폴더를 클릭하고 Next 버튼을 누른다.





---
<!--_color: yellow-->
![width:500](./project_vr/e3.jpg)

###### 4. Open with '해당 버전' 버튼을 누른다.


---
# 폰트 목록

- 사이트: 눈누 https://noonnu.cc/


1. 나눔 바른 고딕
https://noonnu.cc/font_page/36

![h:70](./project_vr/f1.jpg)

2. 나눔고딕코딩
https://noonnu.cc/font_page/40

![h:70](./project_vr/f2.jpg)


---

3. 한림고딕체 
https://noonnu.cc/font_page/877

![h:70](./project_vr/f3_hanrim.jpg)


4. KoddiUD 온고딕
https://noonnu.cc/font_page/674

![h:70](./project_vr/f4_kodd.jpg)
---

5. 예스 고딕
https://noonnu.cc/font_page/404

https://www.relation.co.kr/html_board/board_view.php?par_no=13&code=&title_code=&page=1&no=144


---

- 사이트: Relation 
https://www.relation.co.kr/html_board/board_view.php?par_no=13&code=&title_code=&page=1&no=144

1. ELAND Choice

![w:400](./project_vr/f6_eland.jpg)

###### https://www.relation.co.kr/html_board/board_view.php?par_no=13&code=&title_code=&page=1&no=144

---

2. KOHI 나눔체

![w:400](./project_vr/f7_kohi.jpg)
###### https://www.relation.co.kr/html_board/board_view.php?par_no=13&code=&title_code=&page=1&no=152

---

3. KOHI 나눔체