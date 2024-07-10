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
        <h5>HAProxy 설정</h5>
        <img src="https://github.com/DevelopIsHobby/CCCR_Ansible/assets/107912101/4fc7a34a-8f45-404d-a6c0-5635ca1a4c52" width="350" height="130">
        <h5>HAProxy 서버 IP로 접속</h5>
        <img src="https://github.com/DevelopIsHobby/CCCR_Ansible/assets/107912101/47034694-d5d8-4762-a583-264545b0e459" width="800" height="400"></details>

  <h3>3. 도메인 설정</h3>
    <details>
        <h5>도메인(webserver.com) 설정</h5>
        <img src="https://github.com/DevelopIsHobby/CCCR_Ansible/assets/107912101/84bc0a5d-e0ae-45c3-ad7a-e1869c3c3a50" width="450" height="200">
        <h5>도메인(webserver.com)으로 검색</h5>
        <img src="https://github.com/DevelopIsHobby/CCCR_Ansible/assets/107912101/4b0e99f1-c545-4fd6-976e-688aad5e5c3b" width="800" height="200"></details>

   <h3>4. NFS & iSCSI</h3>
      <details>
        <h5>워드프레스 서버 : NFS 공유폴더안에 있는 /wordpress</h5>
        <img src="https://github.com/DevelopIsHobby/CCCR_Ansible/assets/107912101/d1b9ed50-ed30-4f01-bb78-051c80d52b3b" width="550" height="130">
        <h5>DB 서버 : iSCSI로 제공받은 /dev/sdb에 /db 마운트</h5>
        <img src="https://github.com/DevelopIsHobby/CCCR_Ansible/assets/107912101/0d6d75ce-2541-408e-bec5-76b02581f0ed" width="350" height="90"><br>
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

<h3>6. DB 로드 밸런싱</h3> 
   <details>
       <h5>HAProxy 설정</h5>
       <img src="https://github.com/DevelopIsHobby/CCCR_Ansible/assets/107912101/75f0e744-7a67-4385-b570-38536d7f8d04" width="380" height="180">
       <h5>HAProxy 서버 IP로 핑을 날렸을 때의 응답</h5>
       <img src="https://github.com/DevelopIsHobby/CCCR_Ansible/assets/107912101/397b2271-329f-43b7-8db6-1b0dc165fea4"  width="800" height="300">
    </details>
   </div>
   </div> 
    </div>
    <div align= "center">
    <h2 style="border-bottom: 1px solid #d8dee4; color: #282d33;"> 🛠️ Tech Stacks </h2> <br> 
    <div style="margin: 0 auto; text-align: center;" align= "center">
          <img src="https://img.shields.io/badge/Linux-FCC624?style=plastic&logo=Linux&logoColor=black">
          <img src="https://img.shields.io/badge/Ansible-EE0000?style=plastic&logo=Ansible&logoColor=white">
          </div>
    </div>
<div align="center">
  <h2 style="border-bottom: 1px solid #d8dee4; color: #282d33;">😃 소감 🥲</h2>
    :star:리눅스 프로젝트 땐 DB 로드 밸런싱까지 진행하지 못했는데, 이번엔 모두 진행할 수 있어서 매우 뿌듯하다.<br>
    :star:플레이북을 통해 가상머신을 빠르게 복구할 수 있어서 편리했다.<br>
    :sweat_drops:DNS 서버, 스토리지 서버의 이중화까지 진행하지 못한 부분이 아쉽다..<br>
</div>


<div align= "center">
    <h2 style="border-bottom: 1px solid #d8dee4; color: #282d33;"> 🧑‍💻 Contact me </h2> <br> 
    <div align= "center"> 
        <a href="https://github.com/DevelopIsHobby"> 
            <img src="https://img.shields.io/badge/GitHub-ffffff?style=plastic&logo=GitHub&logoColor=black&link=https://github.com/DevelopIsHobby"> 
        </a>
        <a href=https://www.notion.so/05ab0f771bb5433faebb8061defc48c4?pvs=4> <img src="https://img.shields.io/badge/Notion-000000?style=plastic&logo=Notion&logoColor=white&link=https://www.notion.so/05ab0f771bb5433faebb8061defc48c4?pvs=4"> </a>
          </div>  <br> 
    <div align= "center">  </div> 
</div>


   
