<div align= "center">
    <img src="https://capsule-render.vercel.app/api?type=soft&color=gradient&height=180&text=Hello%20World!&animation=fadeIn&fontColor=ffffff&fontSize=70" />
    </div>
    <div align= "center"> 
    <h2 style="border-bottom: 1px solid #d8dee4; color: #282d33;"> 🐶개발환경 </h2>  
    <div style="font-weight: 700; font-size: 15px; text-align: center; color: #282d33;"> </li>컨트롤 노드 : <b>우분투</b><br></li>제어노드 : <b>CentOS 7</b><br></li>서버 종류 : <b>웹 서버 2개, DB 서버2개, 스토리지 서버 1개, DNS 서버 1개</b><br></li>네트워크 : <b>Nat Network(DNS) + Host Only Network(Web, DB, Storage)</b><br></li></div> 
    </div>
    <div align= "center"> 
    <h2 style="border-bottom: 1px solid #d8dee4; color: #282d33;"> 🧸구현기능 </h2>  
    <div style="font-weight: 700; font-size: 15px; text-align: center; color: #282d33;">
    <i>워드 프레스 생성</i><br>
    <i>워드 프레스 로드 밸런싱</i><br>
    <i>도메인 설정</i><br>
    <i>NFS & iSCSI</i><br>
    <i>DB 이중화</i><br>
    <i>DB 로드 밸런싱</i> <br>
   </div> 
    <h2 style="border-bottom: 1px solid #d8dee4; color: #282d33;">  :paw_prints: 아키텍처 </h2>  
    <div style="font-weight: 700; font-size: 15px; text-align: center; color: #282d33;">
        <img src="https://github.com/DevelopIsHobby/CCCR_Ansible/assets/107912101/e9d8937c-14ef-44a1-ade8-f05227ce1157">
    </div> 
    <div align= "center"> 
    <h2 style="border-bottom: 1px solid #d8dee4; color: #282d33;"> 🌹기능설명 </h2>  
    <div style="font-weight: 700; font-size: 15px; text-align: center; color: #282d33;">
  <h3>1. 워드프레스 생성</h3>
  <details>
  <h5>첫 번째 워드 프레스</h5>    
  <img src="https://github.com/DevelopIsHobby/CCCR_Ansible/assets/107912101/e70f1b95-341e-4cfb-b1c6-e5b3a3b490c3"width="800" height="400" >
  <h5>두 번째 워드 프레스</h5>
  <img src="https://github.com/DevelopIsHobby/CCCR_Ansible/assets/107912101/111dd14e-160b-4303-96d3-bd0a87aec8ac"width="800" height="400" >
    </details>

   <h3>2. 워드프레스 로드 밸런싱</h3>
      <details>
        <img src="https://github.com/DevelopIsHobby/CCCR_Ansible/assets/107912101/4fc7a34a-8f45-404d-a6c0-5635ca1a4c52" width="350" height="130">
        <h5>로드밸런서 서버 IP로 접속</h5>
        <img src="https://github.com/DevelopIsHobby/CCCR_Ansible/assets/107912101/47034694-d5d8-4762-a583-264545b0e459" width="800" height="400"></details>

  <h3>3. 도메인 설정</h3>
    <details>
        <img src="https://github.com/DevelopIsHobby/CCCR_Ansible/assets/107912101/84bc0a5d-e0ae-45c3-ad7a-e1869c3c3a50" width="350" height="130">
        <h5>도메인(webserver.com)으로 검색</h5>
        <img src="https://github.com/DevelopIsHobby/CCCR_Ansible/assets/107912101/4b0e99f1-c545-4fd6-976e-688aad5e5c3b" width="800" height="200"></details>

   <h3>4. NFS & iSCSI</h3>
      <details>
        <h5>워드프레스 서버 : NFS 공유폴더안에 있는 /wordpress</h5>
        <img src="https://github.com/DevelopIsHobby/CCCR_Ansible/assets/107912101/d1b9ed50-ed30-4f01-bb78-051c80d52b3b" width="550" height="130">
        <h5>DB 서버 : iSCSI로 제공받은 /dev/sdb에 /db 마운트</h5>
        <img src="https://github.com/DevelopIsHobby/CCCR_Ansible/assets/107912101/0d6d75ce-2541-408e-bec5-76b02581f0ed" width="350" height="90">
          <img src="https://github.com/DevelopIsHobby/CCCR_Ansible/assets/107912101/93148976-daca-4f5e-ae3d-b14c111ded30" width="600" height="200">
        <h5>DB 서버 : /db로 MariaDB 기본 디렉토리 위치 변경</h5>
        <img src="https://github.com/DevelopIsHobby/CCCR_Ansible/assets/107912101/0a60dd99-7a3e-4860-a0a9-541ddd95b97f" width="350" height="200">
      </details>
   <h3>5. DB 이중화</h3>
      <details>
        <h5>DB 서버 : 데이터베이스 추가 전</h5>
        <img src="https://github.com/DevelopIsHobby/CCCR_Ansible/assets/107912101/a04de574-b438-4989-89a9-7defa0e9024b" width="300" height="200">
        <img src="https://github.com/DevelopIsHobby/CCCR_Ansible/assets/107912101/86d16047-9608-4968-91b0-bd9bf4747634" width="300" height="200">
          <h5>DB 서버 : Slave_test2 데이터베이스 추가 후</h5>
          <img src="https://github.com/DevelopIsHobby/CCCR_Ansible/assets/107912101/975a2d1f-123a-4de9-8c20-395a738a9e4b" width="300" height="320">
          <img src="https://github.com/DevelopIsHobby/CCCR_Ansible/assets/107912101/484aa630-e104-426f-ae82-603ce29097f5" width="300" height="320">
      </details>

<h3>6. 게시글 CRUD</h3> 
   <details>
       <h6>게시글 등록</h6>
          <details><img src="https://github.com/DevelopIsHobby/MyBoard/assets/107912101/e18c5fce-2612-478e-9c1e-1a046fd4c083"  width="800" height="400">
          </details>
    <h6>게시글 수정</h6>
       <details><img src="https://github.com/DevelopIsHobby/MyBoard/assets/107912101/410263ce-ca74-4629-91f1-d06c9e45ecc4"  width="800" height="400">
          </details>
    <h6>게시글 삭제</h6>
              <details><img src="https://github.com/DevelopIsHobby/MyBoard/assets/107912101/2107edc0-2700-4162-9f2c-fe0b0519a610"  width="800" height="400">
          </details>
    </details>
    
   <h3>7. 댓글 CRUD</h3> 
   <details>
    <h6>댓글 등록</h6>
          <details><img src="https://github.com/DevelopIsHobby/MyBoard/assets/107912101/bbdac3ca-1f92-4f5e-bbe7-57632ab1e8dc3"  width="800" height="400">
          </details>
    <h6>댓글 수정 및 삭제</h6>
       <details><img src="https://github.com/DevelopIsHobby/MyBoard/assets/107912101/5bf3b4cb-a0a7-4666-acf4-0e2791157d644"  width="800" height="400">
          </details>
    </details>
   </div>
   </div> 
    </div>
    <div align= "center">
    <h2 style="border-bottom: 1px solid #d8dee4; color: #282d33;"> 🛠️ Tech Stacks </h2> <br> 
    <div style="margin: 0 auto; text-align: center;" align= "center"> <img src="https://img.shields.io/badge/Java-007396?style=plastic&logo=Java&logoColor=white">
          <img src="https://img.shields.io/badge/Spring Boot-6DB33F?style=plastic&logo=Spring Boot&logoColor=white">
          <img src="https://img.shields.io/badge/MariaDB-003545?style=plastic&logo=MariaDB&logoColor=white">
          <img src="https://img.shields.io/badge/Javascript-F7DF1E?style=plastic&logo=Javascript&logoColor=white">
          <img src="https://img.shields.io/badge/jQuery-0769AD?style=plastic&logo=jQuery&logoColor=white">
          <br/><img src="https://img.shields.io/badge/HTML5-E34F26?style=plastic&logo=HTML5&logoColor=white">
          <img src="https://img.shields.io/badge/Bootstrap-7952B3?style=plastic&logo=Bootstrap&logoColor=white">
          </div>
    </div>
<div align="center">
  <h2 style="border-bottom: 1px solid #d8dee4; color: #282d33;">😃 소감 🥲</h2>
    :star:그동안 웹에 대해 공부하면서 넣어보고 싶었던 기능들을 모두 구현해 볼 수 있어서 매우 뿌듯하다.<br>
    :star:JPA와 Gardle을 활용해 볼 수 있어서 좋았다.<br>
    :sweat_drops:무한스크롤에서 위치를 기억시켜 List 버튼을 클릭했을 때 원래 있던 위치로 가게 하는 것을 구현하지 못했다.<br>
    :sweat_drops:스프링 시큐리티 적용 못한 것이 아쉽다.<br>
    :punch:일정 시간 동안 일정 수 이상의 추천을 받을 경우 핫 게시판이 되게 하는 기능도 넣어보고 싶다.
</div>


<div align= "center">
    <h2 style="border-bottom: 1px solid #d8dee4; color: #282d33;"> 🧑‍💻 Contact me </h2> <br> 
    <div align= "center"> <a href=https://www.notion.so/05ab0f771bb5433faebb8061defc48c4?pvs=4> <img src="https://img.shields.io/badge/Notion-000000?style=plastic&logo=Notion&logoColor=white&link=https://www.notion.so/05ab0f771bb5433faebb8061defc48c4?pvs=4"> </a>
          </div>  <br> 
    <div align= "center">  </div> 
</div>


   
