# TIL       
          
           
## 📣notion  이용방법    

(notion 은 노트,일정,업무,데이터,프로젝트 등을 효율적으로 생성하고 관리할 수 있는 All-in-one 생상성 도구이자 협업 툴입니다.)

- 워크스페이스 섹션의 페이지들은 전체 팀이 할 수 있습니다.
- 개인페이지 섹션의 페이지들은 개인(본인)만 확인 할 수 있습니다.
- 개인페이지 섹션의 페이지 추가를 하려면 해당 섹션 페이지 옆에 (+) 버튼으로 추가 할 수 있습니다.
- 글 작성시, "/"를 누르면 명령어를 입력 할 수 있습니다.(토글 목록, 제목, 리스트, 이모지, ... 등등)
- 공유된 페이지 섹션에 있는 페이지는 초대나 권한을 받아야만 확인 할 수 있습니다.
- 해당글이나 문장에 댓글을 남기고 싶을때는 해당 문장 더블클릭 후 댓글 누르면 댓글을 남길 수 있습니다.
- 댓글 작성시 "@"를 누르면 멘션을 추가 할 수 있습니다.
- "ctrl+p" 누르면 검색을 할 수 있습니다.
- 워크스페이스 섹션 중 프로젝트 하위에 일정을 클릭하면 일정을 확인 할 수 있습니다.

## 📣Slack 이용방법

(Slack 은 채널 기반 메시징 플랫폼입니다. 워크스페이스는 채널로 구성되어 있고 팀 멤버가 서로 커뮤니케이션하고 협업 할 수 있는 공간입니다.)

- 채널 섹션에 여러페이지 중 앞쪽에 자물쇠 표시가 있는 페이지는 초대를 받거나 권한을 확인 받아야 이용 할 수 있습니다.
- 다이렉트 메세지 섹션은 메세지를 보낼 수 있는 회원들을 확인 할 수 있습니다. 메세지를 보내기 위해서 해당 멤버를 클릭하면 해당멤버에게 메세지를 전송 할 수 있습니다.
- 대화방에서 "@here" 을 입력 후 메세지를 전송하게 되면 채널의 모든 온라인 멤버에게 알림이 뜹니다.
- 채널의 멤버가 메세지를 보냈을때, 확인했다는 의미로 반응을 추가 할 수 있습니다.

     ex) : 👍 이나 ☑️ .. 등등 여러 이모지로 확인을 뜻하는 반응을 보냅니다.

## 📣Jira 이용방법

(Jira 는 이슈기반의 프로젝트 관리 소프트웨어 입니다. 이슈들은 관리자에 의해 만들어진 프로젝트에 속하게 됩니다.)

- Jira 에 프로젝트를 클릭하여 들어오게 되면 좌측에 메뉴들을 볼 수 있습니다.
- 칸반 보드의 경우 한눈에 일정들을 확인 할 수 있습니다.
- 백로그에 개발하기로 선택됨을 보면 현재 개발을 하면서 필요한 것들이나 해야 할 것들을 확인 할 수 있습니다. 해당 목록 우측에 써있는 것은 ex)MW-193..등등 Git을 이용할때 branch 네임으로 사용하면 됩니다.
- 이슈를 업로드 하고 싶을때는 페이지 상단에 만들기 버튼을 눌러 업로드 할 수 있습니다.
- 이슈 만들기할때 담당자는 미할당으로 클릭하여 업로드 하면 됩니다.(본인이 해야할일 일때는 '나에게 할당'을 클릭하면 됩니다.)
- 이슈 등록 후에 진행중이거나 완료되면 상태 변경해주고 그날그날 무엇을 내용에 써두면 됩니다.

## 📣Ubuntu 에 Mysql 설치하기

- $ lsb_release -a   ㅡㅡ> Ubuntu 버전 확인하기
- $ sudo apt-get update ㅡㅡ> 설치 되어있는 패키지들의 새로운 버젼이 있는지 확인 할 때, 사용가능한 패키지들과 그 버전들의 리스트를 업데이트 하는 명령어, 실제 패키지 버전을 업그레이드하는 것이 아니라 최신 버전 패키지가 있는지를 확인하고 내 우분투에 알려주는 용도.
- $ sudo apt-get install mysql-server ㅡㅡ>  Mysql 설치하기
- $ sudo ufw allow mysql —> mysql 서비스 방화벽 허용하기
- $ sudo ufw deny mysql ㅡㅡ> mysql 서비스 방화벽 막기
- $ sudo ufw allow 3306 ㅡㅡ> mysql의 포트는 3306이기 때문에 해당포트를 허용하기(이미 허용돼 있으면 패스한다고 나옴)
- $ sudo systemctl start mysql ㅡㅡ> mysql 이 설치되었으면 실행해보기
- $ sudo systemctl enable mysql ㅡㅡ> Ubuntu 서버가 재시작 되더라도 mysql이 자동 시작되도록 등록


# 2021.02.05
## 📣APM 서버 프로그램 설치

워드프레스 설치에 필요한 서버 프로그램은 총 3가지. 아래 패키지를 묶어 APM 이라고 합니다.

- Apache : 웹서버
- PHP :  PHP 언어 인터프리터
- MySQL : MySQL 데이터 베이스 서버

## 📣Ubuntu 에 Mysql 설치하기

- $ lsb_release -a   ⇒ Ubuntu 버전 확인하기
- $ sudo apt-get update ⇒ 설치 되어있는 패키지들의 새로운 버젼이 있는지 확인 할 때, 사용가능한 패키지들과 그 버전들의 리스트를 업데이트 하는 명령어, 실제 패키지 버전을 업그레이드하는 것이 아니라 최신 버전 패키지가 있는지를 확인하고 내 우분투에 알려주는 용도.
- $ sudo apt-get install mysql-server ⇒  Mysql 설치하기
- $ sudo ufw allow mysql ⇒ mysql 서비스 방화벽 허용하기
- $ sudo ufw deny mysql ⇒ mysql 서비스 방화벽 막기
- $ sudo ufw allow 3306 ⇒ mysql의 포트는 3306이기 때문에 해당포트를 허용하기(이미 허용돼 있으면 패스한다고 나옴)
- $ sudo systemctl start mysql ⇒ mysql 이 설치되었으면 실행해보기
- $ sudo systemctl enable mysql ⇒ Ubuntu 서버가 재시작 되더라도 mysql이 자동 시작되도록 등록
- $ sudo /usr/bin/mysql -u root -p ⇒ mysql 접속하기

    ---

    (mysql 접속 후)

- SHOW VARIABLES LIKE "%version%"; ⇒ 버전 확인하기
- ALTER USER 'root'@'localhost' IDENTIFIED BY '1027'; ⇒ root 계정에 패스워드 ''1027" 설정하기
- SELECT User, Host, authentication_string FROM mysql.user; ⇒ 현재 mysql의 계정(User)정보를 확인하기
- CREATE DATABASE myplanetdb; ⇒ "myplanetdb"이라는 database 를 만들기
- SHOW DATABASES; ⇒ database 가 잘 만들어졌는지 database 리스트 확인하기
- CREATE USER 'jiyeun'@'localhost' IDENTIFIED BY '1027'; ⇒ 계정은 jiyeun이고 Host는 localhost, 그리고 패스워드는 1027 이라는 myplanetdb를 사용하는 계정을 만들기
- FLUSH PRIVILEGES; ⇒ mysql 의 user 테이블에 추가하거나 변경이 있을 경우 FLUSH PRIVILEGES 쿼리 실행하기
- SELECT User, Host, authentication_string FROM mysql.user; ⇒ user 정보 조회하기
- GRANT ALL PRIVILEGES ON myplanetdb.* to jiyeun@localhost; ⇒ jiyeun 계정에 myplanetdb DB를 사용할 수 있도록 권한을 부여하기
- FLUSH PRIVILEGES; ⇒ 권한을 변경 했으니 FLUSH PRIVILEGES 쿼리
- SHOW GRANTS FOR 'tongchun'@'localhost'; ⇒ jiyeun 계정이 localhost에서 어떤 권한을 가지고 있는지 확인해보기

    ```sql
    GRANT USAGE ON *.* TO `jiyeun`@`localhost`                     
    GRANT ALL PRIVILEGES ON `myplanetdb`.* TO `jiyeun`@`localhost`
    ```

    위 쿼리 결과로 나온 두 건 중 첫번째에 GRANT USAGE ON *.* TO가 있습니다. 이건 *.* 는 아무 권한이 없다는 의미입니다. 현재 jiyeun 계정은 myplanetdb 에만 모든 권한을 가지고 있고 mysql의 admin이나 system을 접근 할 수 있는 권한은 없습니다.

    계정 뒤에 붙은 @[localhost](http://localhost)는 해당 계정이 localhost 즉 mysql이 설치된 pc에서만 접속 할 수 있다는 의미입니다. 만약 다른 서버(remote)에서 접속하고 싶다면 접속하려는 서버의 IP로 계정을 새로 만들어줘야 합니다. 예를 들어 192.168.0.10에서 접속하고 싶다면 아래와 같이 쿼리를 실행하면 됩니다.

```sql
CREATE USER 'root'@'192.168.0.10' IDENTIFIED BY 'ngle1234';

GRANT ALL PRIVILEGES ON * . * TO 'root'@'192.168.0.10' WITH GRANT OPTION; 

FLUSH PRIVILEGES;
```

      만약 특정 PC(192.168.0.10)이 아닌 어디서든 접속하려면 IP대신 %로 해주면 됩니다.

```sql
CREATE USER 'root'@'%' IDENTIFIED BY 'ngle1234';

GRANT ALL PRIVILEGES ON * . * TO 'root'@'%' WITH GRANT OPTION; 

FLUSH PRIVILEGES;
```

- SELECT User, Host, authentication_string FROM mysql.user; ⇒ 계정 리스트를 다시 보면 root@% 계정이 추가 된걸 확인할수 있습니다.
- CREATE USER 'jiyeun'@'%' IDENTIFIED BY '1027';

    GRANT ALL PRIVILEGES ON myplanetdb.* TO 'jiyeun'@'%';

    FLUSH PRIVILEGES; ⇒ 마찬가지로 jiyeun 계정도 remote 접속이 필요해서 실행

## 📣Ubuntu 20.04 에 Apache 설치하기

---

- **Apache 설치**

```basic
$ sudo apt update && sudo apt install apache2
```

⇒ 첫번째 명령은 패키지 목록을 업데이트하고 Apache에 대한 최신 버전과 종속성을 얻을 수 있도록 합니다. 두번째 명령은 Apache를 다운로드하고 설치합니다.

---

- **방화벽 구성**

```basic
$ sudo ufw allow OpenSSH
```

⇒ 서버를 원격으로 구성하는 경우 방화벽을 활성화 할 때 잠기는 것을 원하지 않기 때문에 SSH에 대한 방화벽 규칙을 추가합니다. "오류:openSSH와 일치하는 프로필을 찾을 수 없습니다"라는 오류가 발생 하는 경우 서버를 원격으로 구성하지 않고 무시 할 수 있습니다.

```basic
$ sudo ufw allow in "Apache Full"
$ sudo ufw enable
```

⇒ Apache에 대한 방화벽 규칙을 추가 할 수 있습니다. 방화벽이 활성화되지 않은 경우 활성화합니다.

```basic
$ sudo ufw status
```

⇒ 현재 방화벽 상태를 확인 할 수 있습니다.

---

- **Apache 테스트**

```basic
$ sudo service apache2 status
```

⇒ Apache가 올바르게 설치되었는지 확인하기 위해 현재 Apache 서비스 상태를 확인 할 수 있습니다.

실행중이면 Active 가 녹색으로 표시되어야 합니다.

```basic
$ hostname -I
```

⇒ 본인의 아이피를 확인 할 수 있습니다.

확인된 아이피를 주소 표시줄에 입력하면 Apache default Page 가 나옵니다.

```basic
$ sudo nano /var/www/html/index.html
```

⇒ 기본 시작 페이지를 편집 할 수 있습니다. 종료는 CTRL + X 입니다.

---

- **가상 호스트 구성**

    ```basic
    $ sudo mkdir -p /var/www/mydomain.com/public_html
    ```

    ⇒ Ubuntu 20.04 서버에서 여러 도메인을 호스팅하려면 가상 호스트를 설정해야합니다.

    /var/www/ 도메인에 대한 새 디렉토리를 만듭니다. [mydomain.com](http://mydomain.com) 을 자신의 것으로 바꿉니다.

    ```basic
    $ sudo nano /var/www/mydomain.com/public_html/index.html
    ```

    ⇒ 테스트를 위해 index.html 파일을 만듭니다.

    ```html
    <html>
       <head>
         <title>Welcome!</title>
       </head>
       <body>
          <h1>Welcome to mydomain.com!</h2>
       </body>
    </html>
    ```

    ⇒ 그리고 다음을 입력하고 저장 및 종료(ctrl+x ... y 를 차례로 누르고 enter 을 누릅니다.)

    ```html
    $ sudo nano /etc.apache2/sites-available/mydomain.com.conf
    ```

    ⇒ [mydomain.com](http://mydomain.com) 을 자신의 것으로 대체하는 가상 호스트 구성 파일을 만듭니다.

    ```basic
    <VirtualHost *:80>
        ServerAdmin webmaster@mydomain.com
        ServerName mydomain.com
        ServerAlias www.mydomain.com
        DocumentRoot /var/www/mydomain.com/public_html
        ErrorLog ${APACHE_LOG_DIR}/error.log
        CustomLog ${APACHE_LOG_DIR}/access.log combined
    </VirtualHost>
    ```

    ⇒ 다음을 입력하여 [mydomain.com](http://mydomain.com) 을 자신의 것으로 바꿉니다.

    저장 및 종료(ctrl+x ... y 를 차례로 누르고 enter 을 누릅니다.)

    ```basic
    $ apachectl configtest
    ```

    ⇒ 오류를 테스트 합니다.

    ```basic
    $ sudo a2ensite mydomain.com.conf
    ```

    ⇒ [mydomain.com](http://mydomain.com) 을 자신의 것으로 대체하는 가상 호스트를 활성화합니다.

    ```basic
    $ sudo a2dissite -default
    ```

    ⇒ 기본 Apache 웹 사이트를 비활성화합니다. 그렇지 않으면 가상 호스트를 재정의합니다.

    ```basic
    $ sudo systemctl reload apache2
    ```

    ⇒ Apache 를 다시 시작합니다.

    이제 브라우저에서 사이트를 로드 할 수 있습니다.

    이제 4개의 단계를 반복하여 더 많은 도메인을 추가 할 수 있습니다.
    
    
   # 2021.02.06

# 리눅스 기본 명령어

- 모든 명령어는 명령어 뒤에 "—help" 옵션을 주면 자세한 사용 방법이 나온다.

    ex) Is 명령의 자세한 사용 방법과 모든 옵션을 알고 싶으면 Is-help 를 입력하면 된다.

### pwd(print working directory)

현재 작업중인 디렉토리 정보 출력

```jsx
$ pwd
/home/root
```

### cd ( change directory)

경로 이동

절대 경로와 상대 경로로 이동 가능

```jsx
$ cd /home/root/jiyeun
$ pwd
/home/root/jiyeun

$ cd ..           (상위폴더로)
$ pwd
/home/root
```

### ls ( list )

디렉토리 목록 확인

```jsx
$ ls
testfile1 testfile2 testfile3
```

### cp (copy)

파일 혹은 디렉토리를 복사

디렉토리를 복사할때는 -r 옵션을 주어야함

cp 명령어 뒤에 복사하고자 하는 파일이나 디렉토리적고 복사하는 파일이나 디렉토리 네임

```jsx
$ ls
testdir/ testfile

$ cp testfile1 testfile_cp
$ ls
testdir/ testfile testfile_cp

$ cp -r testdir testdir_cp
$ls
testdir/ testdir_cp/ testfile testfile_cp
```

### mv (move)

파일 혹은 디렉토리 이동

실제로 원하는 위치로 이동할때도 사용하지만, 이름을 변경하는 용도로도 사용한다.

같은 폴더에서 파일, 디렉토리 이동을 하는 경우 이름변경 효과가 있다.

앞에 파일이 오고 뒤에 디렉토리가 오는경우에는 파일을 디렉토리로 이동한다.

여러개의 파일도 이동이 가능하다 ex) mv 파일명 파일명 디렉토리/

cp 와는 달리 디렉토리를 이동할때도 별다른 옵션이 필요없다.

```jsx
$ ls
testdir/ testfile

$ mv testfile testfile_mv  (이름변경)
$ls
testdir/ testfile_mv

$ mv testfile_mv testdir/    (앞에 파일이 오고 뒤에 디렉토리가 오는경우)
$ ls
testdir/

$ ls testdir/
testfile

$ mv dir1/ dir2/    (dir1 디렉토리를 dir2 디렉토리로 이름을 변경)
```

### mkdir ( make directory)

디렉토리 생성

-p 옵션을 주면 하위 디렉토리까지 한 번에 생성 가능

아래 예제중 ls -R 옵션은 디렉토리의 하위목록까지 전부 보여주는 옵션

```jsx
$ mkdir dir1    (현재 디렉토리에 dir1 디렉토리를 만듬)
$ mkdir dir1 dir2   (한번에 여러개의 디렉토리 생성)
$ mkdir -p dir1/dir2  (디렉토리를 만들 때 상위(부모) 디렉토리가 없으면 만든다.
$ mkdir -m 700 dir5    (디렉토리를 만들 때 권한 까지 지정)
```

### rm (remove)

파일이나 디렉토리를 삭제

디렉토리를 삭제할때는 r 옵션을 주어야 한다.

-f 옵션을 주면 사용자에게 삭제 여부를 묻지 않고 바로 삭제한다.

디렉토리를 삭제할 때는 하위 디렉토리까지 모두 삭제되므로 **유의**

rmdir 은 디렉토리를 삭제할때 사용하나 일반적으로 rm -r 을 이용해서 삭제한다.

```jsx
$ ls
testdir/ testfile1 testfile2

$ rm -f testfile1
$ ls
testdir/ testfile2

$ rm -rf testdir/
$ ls
testfile2

$ rm -r home/     (비어있지 않은 디렉토리는 -r 옵션 없이는 삭제 불가능)
```

### touch

파일이나 디렉토리의 최근 업데이트 일자를 현재 시간으로 변경한다.

최근 업데이트 일자는 ls -l 명령을 통해 확인 할 수 있다.

아래 예제에서 '11월 6 22:08' 이라고 쓰여진 부분이다.

파일이나 디렉토리가 존재하지 않으면 빈 파일을 만든다.

-t 라는 옵션을 사용하면 서버의 현재시간이 아닌 지정된 시간으로 파일의 날짜시간 정보를 변경한다.

```jsx
$ ls -l
total 0
-rw-r--r-- 1 jiyeun 197121 0 11월 6 22:08 testfile1

$ touch testfile1
$ ls -l
total 0
-rw-r--r-- 1 jiyeun 197121 0 11월  6 22:43 testfile1
-rw-r--r-- 1 jiyeun 197121 0 11월  6 22:44 testfile2

$ touch newfile   (빈 파일 생성)
$ touch -c newfile (현재시간으로 파일 날짜정보 변경)
$ touch -t 202011141200 newfile (파일의 날짜정보를 마음대로 변경(YYYYMMDDhhmm 형식)
$ touch -r oldfile newfile (지정한 파일 날짜시간정보를 지정한 다른 파일의 날짜시간정보와 
														동일하게 변경(newfile을 oldfile의 날짜정보와 같게 변경))
```

### cat ( concatenate)

cat 명령은 활용방법이 다양하다.

단순히 파일의 내용을 출력 할 수도 있고, 파일 여러개를 합쳐서 하나의 파일로 만들 수도 있다.

그리고 기존 한 파일의 내용을 다른 파일에 덧붙일 수도 있다.

새로운 파일을 만들때에도 사용된다.

file1, file2, file3 파일에는 각각 간단하게 숫자 1, 2, 3 이 적혀있다.

리다이렉션 기호(>)를 사용하여 입력한 내용으로 새로운 파일 만듬

```jsx
$ ls
file1 file2 file3

$ cat file1  ( cat 명령 뒤에 파일 이름을 입력하면 그 파일의 내용 출력)
1
$ cat file2
2
$ cat file3
3

$ cat file1 file2 file3  (여러 개의 파일을 전달하여 파일내용을 연속해서 출력)
1
2
3

$ cat -n file1 file2 file3  ( cat 명령의 n옵션을 사용하면 행 번호를 표시)

$ cat file1 file2 > file1_2  (file1과 file2 내용을 가진 file1_2라는 파일생성)
$ ls
file1 file1_2 file2 file3

$ cat file1_2
1
2

$ cat >> file1 (내용 입력후 ctrl+d 로 저장)
								( > 기호를 사용하면 기존에 있는 파일 내용을 지우고 저장,
									>> 기호를 사용하면 기존 파일 내용 뒤에 연속해서 기록저장)

$ cat file1 >> file2  ( file2 에 file1 내용을 연속해서 기록저장)
$ cat file2
2
1

$ cat > file4 (내용을 입력하고 ctrl+d 로 저장, 입력한 내용으로 새로운파일 생성)
hello
world
(작성이 끝나면 ctrl +d 로 파일 저장)

$ cat file4
hello
world
```

### head

파일의 앞부분을 보고싶은 줄 수 만큼 보여준다.

옵션을 지저어하지 않으면 파일 상위 10줄을 보여준다.

```jsx
$ cat testfile
1
2
3
4
5
6
7
8
9
10
11
12
13
14
15

$ head -3 testfile (-3 으로 범위를 지정했기 때문에 3줄만 나옴)
1
2
3

$ head testfile  (범위를 지정안해서 상위 10줄만 보여줌)
1
2
3
4
5
6
7
8
9
10
```

### tail

파일의 뒷부분을 보고싶은 줄 수 만큼 보여준다.

옵션을 지정하지 않으면 파일 하위 10줄을 보여준다.

참고로 -F 옵션을 주고 실행하면, 

파일내용을 화면에 계속 띄워주고 파일이 변하게되면 새로운 업데이트 된 내용을 갱신해준다.

주로 실시간으로 내용이 추가되는 로그파일을 모니터링할때 유용하게 사용한다.

```jsx
$ cat testfile
1
2
3
4
5
6
7
8
9
10
11
12
13
14
15

$ tail -3 testfile (하위 범위를 정해줌)
13
14
15

$ tail testfile
6
7
8
9
10
11
12
13
14
15

$ tail -F testfile
6
7
8
9
10
11
12
13
14
15
(명령어가 종료되지 않고 계속 해당 화면을 출력하며, 파일 내용 변경시 자동으로 갱신)
```

### find

특정 파일이나 디렉토리를 검색한다.

사용법이 앞의 명령어들에 비해 살짝 복잡. 기본 사용법을 언급하자면 다음과 같다.

find[검색경로] -name [파일명]

파일명은 직접 풀 네임을 입력해도 되지만, 다음 예제처럼 특정 조건을 적용해 검색 할 수도 있다.

```jsx
$ ls
dir1/ dir3/ file1 file3 picture1.jpg picture3.jpg
dir2/  dir4/  file2  file4  picture2.jpg  picture4.jpg

$ find ./ -name 'file1'
./file1

$ find ./ -name "*.jpg" (.jpg 인 파일을 찾는것)
./picture1.jpg
./picture2.jpg
./picture3.jpg
./picture4.jpg
```

확장자가 .jpg 인 파일을 찾았다.

하지만 여기서 그치지 않고, 확장자가 .jpg인 파일만 찾아서 바로 삭제 할 수도 있다.

exec 옵션을 사용해 다음과 같이 처리한다.

```jsx
$ find ./ -name "*.jpg" -exec rm {} \;
$ ls
dir1/  dir2/  dir3/  dir4/  file1  file2  file3  file4
```

-type 옵션을 주면, 디렉토리나 파일만 지정해서 검색 할 수도 있다.

```jsx
$ find ./ -type d
./
./dir1
./dir2
./dir3
./dir4

$ find ./ -type f
./file1
./file2
./file3
./file4
```

wc -l 옵션과 같이 사용하면,

특정 디렉토리에 find 조건에 맞는 결과 값이 몇 개 존재하는지 숫자로 간편히 알아볼 수 있다.

```jsx
$ find ./ -type f | wc -l
4
```

아래 내용은 명령어가 조금 복잡하지만,

특정 조건에 해당하는 파일들의 내용을 전부 찾아서 바꾸는 것이다.

예를 들어, 10만개의 파일이 있는데, 그 중에 확장자가 .txt 인 파일만 찾아내고,

txt 파일 안에 있는 'hi' 라는 문자열을 'hello'로 바꾸려면 다음과 같이 하면 된다.

```jsx
$ find ./ -name "*.txt" -exec sed -i 's/hi/hello/g' {} \;
(sed 명령어는 testfile1.txt 이라는 파일의 모든 hi 라는 문자열을 hello로 바꾸는 역할)

$ sed -i 's/hi/hello/g' testfile1.txt
(이를 find 명령과 조합하여 조건에 맞는 모든 파일에 대해 해당 명령을 수행할 수 있도록 응용한것)
```



## 2021.02.08
## 📣Ubuntu 20.04 에 Uginx 설치 및 최적화

```jsx
sudo apt update && apt upgrade -y
```

      시작전 기본패키지 업데이트 및 최신화합니다.

```jsx
sudo apt install curl gnupg2 ca-certificates lsb-release
```

      nginx 패키지 설치이전 선행작업

```jsx
sudo apt update
sudo apt install nginx
```

      레포지토리의 최신 버전이 설치 됩니다.

```jsx
sudo service nginx start
service nginx status
nginx -v
```

      설치가 완료 되면 버전을 확인해줍니다.

```jsx
sudo netstat -lntp
```

      nginx 구동테스를 위해 80번 포트가 리스닝 되고있으면 실행이 된 상태입니다.

웹으로 접근하려면 브라우저에서 ip를 넣어주면 됩니다.

```jsx
sudo systemctl enable nginx.service
```

      재부팅시 자동시작을 위해 서비스를 등록합니다.

nginx 의 설정 파일은 /etc/nginx/nginx.conf 입니다.

기본적으로 nginx의 Process 구조는 아래와 같습니다.

apache 는 스레드, 프로세스 기반의 아키텍처인 반면에 

nginx의 경우 이벤트 중심에 아키텍처가 있습니다.

nginx는 다수의 작업자 프로세스를 실행할 수 있으며, 각각은 다수의 동시 연결을 처리 할 수 있습니다.

worker_processes – Nginx 작업자 프로세스 수 (기본값은 1).대부분의 경우 CPU 코어 당 하나의 작업자 프로세스를 실행하면 효과가 있으며, 이를 달성하기 위해이 지정 문을 설정하는 것이 좋습니다 .작업자 프로세스가 많은 디스크 I / O를 수행해야하는 경우,이 수를 늘리려는 경우가 있습니다.

worker_connections – 각 작업자 프로세스가 동시에 처리 할 수있는 최대 연결 수.기본값은 512이지만 대부분의 시스템에는 더 많은 수를 지원하기에충분한 리소스가 있습니다.적절한 설정은 서버 크기와 트래픽 특성에 따라 다르며테스트를 통해 검색 할 수 있습니다.

```jsx
sudo vi /etc/nginx/nginx.conf
```

      로 들어가 아래 부분과 같이 변경해주세요

```jsx
worker_processes 4;
events {
worker_connections 1024;
}
```

      설정 후 sudo service nginx restart 로 재시작을 해줍니다.

## 📣PHP-FPM 설치 및 설정

      nginx 에서 php파일을 읽을 수 있도록 php-fpm 을 설치해보도록 하겠습니다.

php-fpm 설치는 매우 단순하나 nginx설정을 비롯해서 최적화 과정이 복잡하기 때문에 잘 따라와야한다.

```jsx
sudo apt install -y php7.4-fpm php7.4-gd php7.4-json php7.4-mysql
php7.4-curl php7.4-mbstring php7.4-intl php-imagick php7.4-xml php7.4-zip
```

      입력하여 설치를 합니다.

```jsx
php -v
```

      설치가 완료 되었으면 php -v 명령어를 입력하면 설치확인이 가능합니다.

```jsx
sudo vi /etc/php/7.4/fpm/pool.d/www.conf
```

      의 내용중에 listen= 을 찾아서 수정하면 됩니다.

listen = /run/php/php7.4-fpm.sock

바로 밑에 줄에

listen = 127.0.0.1:9000을 입력해주면 됩니다.

```jsx
sudo systemctl restart php7.4-fpm.service
netstat -lntp
```

      재시작 후에 수신확인하기

```jsx
sudo vi /etx/php/7.4/fpm/pool.d/www.conf
```

       들어가서 /pm = dynamic 으로 찾고 아래와 같이 수정해줍니다.

```jsx
pm.max_children = 120
pm.start_servers = 12
pm.min_spare_servers = 6
pm.max_spare_servers = 18
```

```jsx
sudo systemctl restart php7.4-fpm.service
ps -ef | grep php
```

      설정 완료후에 재시작 시켜주고 확인하면 변경된걸 확인 할 수 있습니다.

```jsx
sudo vi /etc/php/7.4/fpm/php.ini
```

      php 최적화(메모리 및 업로드 크기)를 위해서 파일로 들어간 후에

```jsx
memory_limit = 1024M
post_max_size = 128M
upload_max_filesize = 128M
```

      수정해주면 됩니다. (메모리,용량은 용도에 맞춰서 설정하시면 됩니다.)

변경 후에 다시 sudo systemctl restart php7.4-fpm.service 명령어로 다시 시작하고 

확인해주면 됩니다.

```jsx
sudo vi /etc/nginx/sites-available/default
```

      nginx는 설정파일을 변경해야 합니다.

`upstream php-handler {server 127.0.0.1:9000;}`

`server {client_max_body_size 128M;listen 80 default_server;listen [::]:80 default_server;`

`root /var/www/html;`

`index index.php index.html index.htm index.nginx-debian.html;`

`server_name _;`

`access_log /var/log/nginx/web.access.log;error_log /var/log/nginx/web.error.log;`

`location / {`

`try_files $uri $uri/ /index.php?$args;}`

`error_page 404 /404.html;`

`error_page 500 502 503 504 /50x.html;`

`location = /50x.html {root /usr/share/nginx/html;}`

`location ~ \.php$ {fastcgi_pass php-handler;fastcgi_param SCRIPT_FILENAME $document_root$fastcgi_script_name;include fastcgi_params; fastcgi_read_timeout 300;}`

`location ~ /\.ht {deny all;}}`

## 📣 워드프레스 설치

```jsx
wget https://wordpress.org/latest.tar.gz
```

 wget 명령어를 이용하여 워드프레스를 다운받습니다.

```jsx
gzip -d latest.tar.gz && tar xvf latest.tar
```

압축파일로 다운받아지기 때문에 압축을 해제해 줍니다.

압축을 풀면 wordpress 란 디렉터리에 파일이 모두 압축해제 되어있는것을 알수있습니다.

```jsx
rm -rf /var/www/html/*
cp -r /root/wordpress/* /var/www/html/
```

이것을 웹 투트 디렉터리로 이동시켜줍니다.

## 📣웹 접속 후 설정하기

웹으로 ip에 접속해보면 잘 나올것이다. 여기서 let's go 버튼을 누르면 db정보를 입력하는데

제출하면 이번에는 wp-config 에 해당 내용을 복사 붙여넣기 하라고 한다.

vi /var/www/html/wp-config.php 하여 새로 만들어서 복사 붙여넣기 하면 된다.

그리고 Run the installation 하면 사이트 설정을 하고 마무리한다.

---

---

## 📣Ubuntu 에서 notion 설치

([https://tolovefeels.tistory.com/63](https://tolovefeels.tistory.com/63) 을 참고)

```
wget https://notion.davidbailey.codes/notion-linux.list
sudo mv notion-linux.list /etc/apt/sources.list.d/notion-linux.list
sudo apt update && sudo apt install notion-desktop
```

```jsx
npm -g install asar electron-packager electron-installer-debian
```

1. nvm 을 이용하여 node 를 설치해줍니다

    `nvm install node`

2. npm 버전 7 을 설치합니다.

    `npm install -g npm@7`

3. 앱 빌드에 필요한 다른 패키지를 설치합니다.(apt사용)

    `sudo apt install p7zip-full imagemagick make g++ fakeroot rpm`
    

# 2021.02.09
## 📣 가상 머신(VM) 이란?

컴퓨터 안에 또 다른 컴퓨터를 동작 시키는 것이다. 컴퓨터 시스템을 에뮬레이션 한다고 말한다.

이를 종종 게스트라고 하며, 이를 실행하는 실제 시스템을 호스트라고 한다.

실제로 물리적으로 존재는 컴퓨터는 아니지만 실제 컴퓨터처럼 작동한다.

컴퓨터의 주된 부붐들(CPU, RAM, 하드디스크 등)의 기능을 소프트웨어적으로 구현해 가상으로 만들어서    

구현한다.

가상 머신은 크게 시스템 가상 머신과 프로세스 가상 머신 두 가지로 나뉜다.

시스템 가상 머신은 실제 기계를 대체해서 제공하며, 전체 운영체제를 실행하기 위한 기능들을 제공한다.

프로세스 가상 머신은 플랫폼에 독립적인 환경에서 컴퓨터 프로그램을 실행하기 위해 고안되었다. 프로그

래밍언어의 하드웨어 추상화를 위해 사용된다.

가상화를 이용하면 하나의 물리적 시스템에서 각각 자체 운영 체제(OS)와 애플리케이션을 지닌 다수의

가상머신을 작성 할 수 있다. VM은 실제 컴퓨터와 직접 상호 작용 할 수 없다.

대신에 여기서 VM과 기본적인 실제 하드웨어 간의 조정을 위해 하이퍼바이저라고 하는 경량 소프트웨어

계층이 필요하다. 하이퍼바이저는 실제 컴퓨팅 리소스(예: 프로세서,메모리 및 스토리지)를 각 VM에

할당한다. 이는 서로 간에 간섭하지 않도록 VM을 각각 분리한다.

이 기술은 가상 서버, 가상 서버 인스턴스(VSI)및 가상 프라이빗 서버(VPS)등을 포함하여 많은 이름으로

불리기도 한다.

## 📣하이퍼바이저란?

하이퍼바이저는 호스트 컴퓨터에서 다수의 운영체제를 동시에 실행하기 위한 논리적 플랫폼을 말한다. 가상화 머신 모니터 또는 가상화 머신 매니저라고도 부른다.

하이퍼바이저는 일반적으로 2가지로 나뉜다.

- 타입 1

운영 체제가 프로그램을 제어하듯이 하이퍼바이저가 해당 하드웨어에서 직접 실행되며 게스트 운영 체제는 하드웨어 위에서 2번째 수준으로 실행된다.

- 타입2

하이퍼바이저는 일반 프로그램과 같이 호스트 운영 체제에서 실행되며 VM 내부에서 동작되는 게스트 운영 체제는 하드웨어에서 3번째 수준으로 실행된다.

## 📣AWS 에서 워드프레스

- 1단계 : Amazon Machine Image 선택

(사진1)EC2 인스턴스를 생성하려면 AWS 콘솔에서 Amazon EC2로 이동한다. [인스턴스 시작] 이라고 적힌 파란색 버튼을 클릭하여 인스턴스 생성 마법사를 연다.

(사진1)

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/8795014f-2b14-4a49-ae3c-1f27a03b9891/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/8795014f-2b14-4a49-ae3c-1f27a03b9891/Untitled.png)

(사진2)첫 페이지에서 Amazon Machine Image("AMI")를 선택한다. 선택하는 AMI에 따라 새 EC2 인스턴스에 설치되는 기본 소프트웨어가 결정된다. 여기에는 운영체제(예: Amazon Linux, Red Hat Enterprise Linux, Ubuntu, Microsoft Server 등)는 물론이고, 머신에 설치되는 애플리케이션도 포함된다.

많은 AMI는 다양한 애플리케이션을 실행하기 위한 범용 AMI이지만 딥 러닝 AMI나 다양한 AWS Marketplace AMI를 비롯한 일부 AMI는 특정 사용 사례에 맞게 특별히 구축된 AMI 이다.

Amazon Linux  배포판을 선택하는 것이 일반적이므로 AMI 선택 뷰에서 Amazon Linux 2 AMI(HVM)를 선택한다.

(사진2)

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/375beb73-c86f-452f-995a-086b6a08a1eb/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/375beb73-c86f-452f-995a-086b6a08a1eb/Untitled.png)

- 2단계 : 인스턴스 유형 선택

(사진3) EC2 마법사의 두 번째 화면에서는 EC2 인스턴스 유형을 선택한다. 인스턴스 유형은 CPU, 메모리(RAM), 스토리지 및 네트워크 용량이 포함된 특정한 구성이다.

AWS에는 여러 가지 워크로드를 포괄하는 수많은 인스턴스 유형이 있다. 어떤 인스턴스는 데이터베이스나 캐시처럼 메모리를 많이 사용하는 워크로드에 적절하고, 어떤 인스턴스는 이미지 처리나 비디오 인코딩처럼 컴퓨팅을 많이 사용하는 워크로드에 적절하다.

(사진3)

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/5a3de5db-3fad-4438-bef2-e0028df1f87a/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/5a3de5db-3fad-4438-bef2-e0028df1f87a/Untitled.png)

- 3단계 : 보안 그룹 구성

(사진4) [검토 및 시작] 버튼을 클릭하면 [인스턴스 시작 검토] 화면이 표시된다. 인스턴스를 시작하기 전에 한가지를 더 구성해야 한다. 보안 그룹은 EC2 인스턴스에 허용되는 네트워크 트래픽 종류를 설명하는 네트워킹 규칙이다. 인스턴스에 다음 두 가지 종류의 트래픽을 허용 할 수 있다.

(사진4)

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/1a406af4-3c07-411b-8f24-163742bc9d8b/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/1a406af4-3c07-411b-8f24-163742bc9d8b/Untitled.png)

(사진5)

🗨️ SSH : SSH 프로토콜을 사용하여 EC2 인스턴스에 로그인하고 WordPress를 구성 할 수 있도록 현재 IP 주소에서 들어오는 SSH 트래픽을 허용한다.

🗨️ HTTP : 사용자가 WordPress 사이트를 볼 수 있도록 모든 IP 주소에서 들어오는 HTTP 트래픽을 허용한다. 이를 구성하려면 검토 페이지에서 [보안 그룹 편집] 링크를 클릭한다.

보안 그룹의 현재 규칙이 표시된다.

SSH 규칙이 구성되어 있지만 모든 IP 주소에서의 SSH 액세스가 허용된다.

HTTP 트래픽을 허용하려면 [규칙 추가] 을 클릭하여 새 규칙에서 [유형] 열의 드롭다운을 클릭해서

HTTP를 선택하면 HTTP 규칙에 대한 기본값이 자동으로 채워진다.

(사진5)

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/236ea56e-8b7b-48a3-b514-ccb2d9288710/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/236ea56e-8b7b-48a3-b514-ccb2d9288710/Untitled.png)

- 4단계 : 시작 및 SSH 키 받기

(사진6)이제 EC2 인스턴스를 시작해야 한다. 파란색 [시작]버튼을 클린하여 EC2 인스턴스를 생성한다.

(사진6)

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/80bbef1d-7808-467d-b91b-e09f7c24ef4a/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/80bbef1d-7808-467d-b91b-e09f7c24ef4a/Untitled.png)

(사진7,사진8)인스턴스의 키 페어를 구성하는 방법이 자세히 표시된다. 키 페어를 사용하여 인스턴스에 SSH를 통해 액세스하면 서버에서 명령을 실행 할 수 있게 된다.

인스턴스의 새 키 페어를 생성하고 이름을 지정한다. 그런 다음 [키 페어 다운로드] 버튼을 클릭하여 머신에 .pem 파일을 다운로드한다. 이 파일은 다음 모듈에서 사용한다.

(사진7)

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/a798c547-c7ae-4bfe-94ce-55a27b12fb50/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/a798c547-c7ae-4bfe-94ce-55a27b12fb50/Untitled.png)

(사진8)

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/ea4a883b-41ec-436b-bce7-5ef12ab3b0a0/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/ea4a883b-41ec-436b-bce7-5ef12ab3b0a0/Untitled.png)

## 📣 EC2 에서 WordPress 구성

- 1단계 : Uginx 웹 서버 설치

Wordpress를 실행하려면 EC2 인스턴스에서 웹 서버를 실행해야 한다.

EC2 인스턴스에 Nginx를 설치하려면 터미널에 명령을 실행한다.

```jsx
ssh -i ~/다운로드/test01.pem ubuntu@52.79.241.25
sudo apt update && apt upgrade -y
sudo apt install curl gnupg2 ca-certificates lsb-release
sudo apt update
sudo apt install nginx
sudo service nginx start
service nginx status
nginx -v
```

(2021.02.05, 2021.02.08 페이지 참조)

- 2단계 : mysql 설치
- 3단계 : php 설치
- 4단계 : wordpress 설치

## 📣 Ubuntu 에서 Mysql 또는 MariaDB 완전 삭제하기

mysql

```jsx
sudo apt-get purge mysql-server
sudo apt-get purge mysql-common
```

mariaDB

```jsx
sudo apt-get purge mariadb-server
sudo apt-get purge mariadb-common
```

공통

```jsx
sudo rm -rf /var/log/mysql
sudo rm -rf /var/log/mysql.*
sudo rm -rf /var/lib/mysql
sudo rm -rf /etc/mysql
```

# 2021.02.10
## 📣 mysql 버전비교

**Stable Version** 은 최종 버전 중에서 테스트가 완료되고 버그가 수정된 안정된 버전이다.

**Legacy Version** 은 아직 사용이 가능한 예전 버전이다. 최신 버전에서 새로 생긴 기능들은 제공되지 않지만 아직까지 최신 환경에서 사용하기에 문제가 없는 버전을 가리킨다.

## 📣 Docker 란

1. 원하는 개발 환경을 파일에 저장하면, docker는 이를 사용자가 원하는 어떤 머신에든 해당 환경을 시뮬레이션 해준다.
2. 이러한 환경들은 각기 독립적으로 존재하기 때문에 원하는 무슨 환경이든 모듈식으로 관리 가능하다. 그래서 예를들어 파이썬서버, 자바서버, 데이터베이스서버 등등 이렇게 추가해서 할 필요 없이 모든 독립적 운용을 docker 하나면 가능하다.
3. 도커는 환경설정을 컨테이너로 분리해 독립된 업무환경을 편하게 도커허브에 도커이미지라는 형태로 백업할 수 있다.
도커와 가상머신의 차이점은 가상머신은 각각의 OS들이 물리적 자원을 분할해서 쓰기때문에 성능저하가 일어나는데, 도커는 OS단까지 가지않고 실행환경만 독립적으로 돌리는거라 가볍고 빠르게 사용할수있다.

## **Docker**

Docker : **컨테이너 기반의 오픈소스 가상화 플랫폼**

- 컨테이너라 하면 배에 싣는 네모난 화물 수송용 박스를 생각할 수 있는데 각각의 컨테이너 안에는

옷,신발,전자제품,술,과일 등 다양한 화물을 넣을 수 있고 규격화되어 다양한 운송수단으로 쉽게 옮길 수 있습니다.

- 다양한 프로그램, 실행환경을 **컨테이너로 추상화하고 동일한 인터페이스**를 제공 => 프로그램의 배포 및 관리를 단순
- 데이터베이스 서버, 자바서버 등 어떤 프로그램도 컨테이너로 추상화 가능.<br>조립PC, AWS, Google cloud등 어디에서든 실행 할 수 있음.

### **컨테이너(Container)란?**

- 컨테이너는 격리된 공간에서 프로세스가 동작하는 기술(가상화 기술의 하나지만 기존 방식과는 차이)

기존의 가상화 방식은 주로 **OS를 가상화**

- VMware 나 VirtualBox 같은 가상머신은 호스트 OS위에 게스트 OS전체를 가상화하여 사용하는 방식.

이 방식은 여러가지 OS를 가상화(ex:리눅스에서 윈도우를 돌리는것)할 수 있고 비교적 사용법이 간단하지만 무겁고 느려서 운영환경에선 사용이 어려움.(각각의 OS들이 물리적 자원을 분할해서 쓰기때문에 성능저하)

이를 개선하기 위해 **프로세스를 격리** 하는 방식이 등장.

리눅스에서는 이 방식을 리눅스 컨테이너라고 하고 단순히 프로세스를 격리시키기 때문에 가볍고 빠르게 동작.

CPU 나 메모리는 프로세스가 필요한 만큼만 추가로 사용하고 성능적으로도 거의 손실이 없음.

- 하나의 서버에 여러개의 컨테이너를 실행하면 서로 영향을 미치지 않고 독립적으로 실행되어 마치 가벼운 VM을 사용하는 느낌.
- 실행중인 컨테이너에 접속하여 명령어를 입력 가능. 패키지를 설치 가능.
- 새로운 컨테이너를 만드는게 걸리는 시간은 1-2초로 가상머신과 비교도 할 수 없이 빠름.

### **이미지(image)란?**

- 도커에서 가장 중요한 개념은 컨테이너와 함게 이미지라는 개념.
- 이미지는 **컨테이너 실행에 필요한 파일과 설정값등을 포함하고 있는 것** => 상태값을 가지지 않고 변하지 않음.
- 컨테이너는 이미지를 실행한 상태라고 볼 수 있고 추가되거나 변하는 값은 컨테이너에 저장.
- 같은 이미지에서 여러개의 컨테이너 생성가능. 컨테이너의 상태가 바뀌거나 컨테이너가 삭제되더라도 이미지는 변하지 않고 그대로 남아있음.
- ubuntu이미지는 ubuntu를 실행하기 위한 모든 파일을 가지고 있고 MYSQL 이미지는 MYSQL을 실행하는데 필요한 파일과 실행 명령어, 포트 정보등을 가지고 있음.
- 이미지는 컨테이너를 실행하기 위한 모든 정보를 가지고 있기 때문에 더이상 의존성파일을 컴파일하고 설치할 필요가 없음. ex) 새로운 서버가 추가되면 미리 만들어 놓은 이미지를 다운받고 컨테이너를 생성하면 됨.
- 한 서버에 여러개의 컨테이너 실행이 가능, 수십,수백,수천대의 서버도 문제없음.
- 도커 이미지의 용량은 거대하고 메가에서 시작해서 기가단위로 넘어가는 경우도 있음.이런 큰 용량의 이미지를 Docker hub를 통해 공개 이미지를 무료로 관리 할 수 있음.


## 📣 Node 지우기

docker 를 설치한 후 node 버전이 원하던 버전과 맞지 않아서 제거

(특정 node.js 버전 삭제하기 $ nvm uninstall vx.x.x 이 방법으로 지우려고 했으나.... 지워지지 않아 

```
sudo apt-get purge nodejs
sudo apt-get autoremove
```

이 명령어로 지우려고 했으나...또 실패...구글링으로 여러 시도를 해보았지만 지워지지 않았다....후...내시간......ㅂㅂ... 하지만!! 방법을 찾음!!!!!!)

```jsx
sudo rm -rf ~/.npm ~/.nvm ~/node_modules ~/.node-gyp ~/.npmrc ~/.node_repl_history

sudo rm -rf /usr/local/bin/npm /usr/local/bin/node-debug /usr/local/bin/node /usr/local/bin/node-gyp

sudo rm -rf /usr/local/share/man/man1/node* /usr/local/share/man/man1/npm*

sudo rm -rf /usr/local/include/node /usr/local/include/node_modules

sudo rm -rf /usr/local/lib/node /usr/local/lib/node_modules /usr/local/lib/dtrace/node.d

sudo rm -rf /opt/local/include/node /opt/local/bin/node /opt/local/lib/node

sudo rm -rf /usr/local/share/doc/node

sudo rm -rf /usr/local/share/systemtap/tapset/node.stp
```

제거 후에 다시 node 를 원하는 버전으로 설치

13.x 로 설치할 예정이며 다른버전을 설치하고싶으시면 앞에 숫자만 변경하시면 됩니다.

```jsx
# Using Ubuntu
curl -sL https://deb.nodesource.com/setup_13.x | sudo -E bash -
```

아래 명령어를 이용하면 위에 등록한 레포지터리에서 node.js를 설치하게 됩니다.

```jsx
sudo apt-get install -y nodejs
```

설치후에 버전은 node -v 명령어로 확인이 가능(node -v 명령어로 확인하려 했으나 오류가 떠서 구글링을 하던 중 해결이 되지 않아 terminal 을 껐다 켰더니 바로 확인됨.......하..내시간) 

```jsx
node -v
```


![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/fff7480e-6396-48f8-9c2c-800aae9d2404/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/fff7480e-6396-48f8-9c2c-800aae9d2404/Untitled.png)

### 도커와 가상머신의 차이점

도커를 이용한 시스템은 호스트OS에서 그대로 작업이 처리되는데 반해 가상머신을 이용한 경우는 중간에 있는 게스트OS에 의해 또 다시 제어되는걸 볼 수 있다. 하드웨어를 가상화하고 운영체제를 가상화하는곳 자체가 없기 때문에 메모리 접근속도, 파일시스템 사용속도, 네트워크 속도 등에서 가상머신에 비해 월등하게 빠른 속도를 가진다.

### 도커의 특징

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/72a3ce75-854d-48e3-9232-99509dc68d2a/Untitled.jpeg](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/72a3ce75-854d-48e3-9232-99509dc68d2a/Untitled.jpeg)

도커는 게스트 OS를 설치하지 않는다.
- 이미지에 서버 운영을 위한 실행 파일과 라이브러리만 격리해서 설치한다.
- OS설치가 없기 때문에 이미지 용량이 크게 줄어든다.
- HOST와 OS자원을 공유한다.

도커에는 하드웨어 가상화 계층이 없다.
- 메모리 접근, 네트워크 전송 속도가 기존의 가상 머신보다 압도적으로 빠르다.
- Host PC와 도커 컨테이너는 성능 차이가 거의 없다. 도커는 이미지 생성과 배포에 특화되어있다.
- Git과 같은 소스 형상관리처럼 이미지 버전 관리도 제공하고, 중앙 저장소에 이미지를 올리고 받을 수 있다.
- GitHub와 비슷하게 도커 이미지를 공유하는 Docker Hub를 제공한다.
- 다양한 API를 제공해서 사용자가 필요한 만큼 자동화가 가능하기 때문에 개발을 할때나 서버 운영을 할 때 매우 유용하다.


## 📣Node 설치 후 VSCODE

node js 는 chrome V8 javascript 엔진으로 빌드된 javascript 런타임입니다.

vscode에 빈프로젝트를 만들고 터미널을 열어줍니다.

express 를 이용할 것이기 때문에 express 사이트로 이동하여 시작하기 탭을 눌러서 들어가 줍니다.

```jsx
npm init
```

명령어를 이용하여 변경하지 않고 그냥 default 값으로 두겠습니다.

```jsx
npm install express --save
```

명령어를 이용하여 express(node.js를 위한 웹프레임워크의 하나)를 설치 하게 되면 관련된 node 모듈이 설치되고

package.json 파일에 셋팅이 됩니다. 이상태에서 new file 을 해서 app.js 라는 이름으로 파일을 만들어줍니다. 

그리고 app.js 에 express 를 연결해주고 원하는 port 번호를 지정한뒤

express().get("/", (req,res) ⇒ res.send("OK"))) get 방식으로 req들어왔을때 OK라는 문자를 res 할 수 있도록 합니다.

app.js 라는 파일을 돌리기 위해서 package.json 파일에서 "scripts" :{ "start" : "node app.js" } 로 변경한뒤 터미널에서 npm start 를 하면 서버가 running 되는 것을 확인 할 수 있습니다.

url 에 [localhost](http://localhost)을 연결해보면 OK가 나옵니다! 이러면 아주 간단하게 웹서버를 킨것입니다.

🤚🏻잠깐! 여기서 연결이 안된다면!

```jsx
sudo netstat -nap|grep 80
```

으로 지금 80번 포트가 이용중인지 확인을 해봅니다

Listen으로 80포트가 사용중이라면 

```jsx
sudo kill $(sudo lsof -t -i:80)
```

이 명령어로 비활성화 시킨뒤에 다시 sudo npm start 를 하면 됩니다!

## 📣docker 를 이용하여 image 만들기

도커는 이미지 기반이기 때문에 컨테이너가 있고 이미지가 들어갑니다.

그래서 지금 만든 OK 웹어플리케이션을 image를 만들어야합니다. 그러기 위해선 image를 만드는것이 dockerfile이 됩니다. vscode 에서 new file로 dockerfile 이라는 이름으로 파일을 만들어줍니다.

그 파일 안에 docker 명령어 들이 들어가야 합니다.

```jsx
FROM node:current-slim
# 이 이미지를 무슨 기반으로 만들것이냐 (부모가 되는 이미지) : 버전은 무엇을 쓰겠냐
# slim 버전은 노드를 실행하기 위해서 최소한의 패키지만을 포함한 버전

WORKDIR /app
#이 프로젝트가 들어갈 워크디렉터리

COPY package.json .
# 이 도커 파일에 위치한 것에 package.json 파일을 copy 하겠다 도커 컨테이너 안에 있는 노드 기반의 컨테이너에 이 앱 디렉토리 안에서 package.json을 복사하겠다

RUN npm install
# 패키지파일 json을 가지고 npm install 을 하면 express 가 설치

EXPOSE 80
# 80 포트를 열겠다

CMD [ "npm", "start" ]
#package.json를 보면 npm start 로 서버를 구동시킴

COPY . .
#남아있는 소스 코드를 복사하겠다
```

dockerfile에 넣어줍니다. 

그리고 터미널에 docker image ls 를 치면 지금은 아무것도 나오지 않을것입니다.(image가 없다는것)

터미널에

```jsx
sudo docker build -t --ok-node-test:0.0.1 .
(이미지태그이름 , 버전, 경로 )
```

이제 node 를 먼저 다운을 받습니다. 이것은 dockerhub 라는 곳에서 다운을 받는것입니다.

```jsx
sudo docker image ls
```

로 다시한번 image 를 확인하면 이미지가 생긴것을 확인 할 수 있습니다. 그런데 여기서 두개인 이유는

부모가 되는 node current slim라는 버전을 받아서 이미지가 있는것이고 , 이 이미지를 기반으로 한 ok-node-test 가 생성된것입니다.

## 📣 AWS 인스턴스 생성 및 접속

aws 에서 인스턴스 생성을 해주고 터미널에서 접속해줍니다.

참고) 2021.02.09

aws 에 도커를 설치해줍니다.

```jsx
sudo apt update && sudo apt -y upgrade
sudo apt install -y apt-transport-https ca-certificates curl gnupg-agent software-properties-common
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"
sudo apt update
sudo apt install -y docker-ce docker-ce-cli containerd.io
```

이렇게 최신 도커 엔진을 설치해주었습니다.

aws 인스턴스에서도 마찬가지로 도커 엔진이 설치 됐는지 확인을 위해

```jsx
sudo docker run hello-world
```

로 확인하겠습니다.

```jsx
Unable to find image 'hello-world:latest' locally

latest: Pulling from library/hello-world

0e03bdcc26d7: Pull complete

Digest: sha256:49a1c8800c94df04e9658809b006fd8a686cab8028d33cfba2cc049724254202

Status: Downloaded newer image for hello-world:latest

Hello from Docker!

This message shows that your installation appears to be working correctly.

To generate this message, Docker took the following steps:

 1. The Docker client contacted the Docker daemon.

 2. The Docker daemon pulled the "hello-world" image from the Docker Hub.

    (amd64)

 3. The Docker daemon created a new container from that image which runs the

    executable that produces the output you are currently reading.

 4. The Docker daemon streamed that output to the Docker client, which sent it

    to your terminal.

To try something more ambitious, you can run an Ubuntu container with:

 $ docker run -it ubuntu bash

Share images, automate workflows, and more with a free Docker ID:

 https://hub.docker.com/

For more examples and ideas, visit:

 https://docs.docker.com/get-started/
```

이런 내용이 나오면 성공입니다.

## 📣dockerhub 에 image 등록하기

dockerhub 에 접속하여 가입을 해서 이메일에서 확인까지 해줍니다.

그리고 myprofile 에 들어가면 repositories 가 비어있는것을 확인할수있습니다.

이제 터미널에서 docker 에 로그인을 해주겠습니다.

```jsx
sudo docker login
```

명령어를 사용하면 username과 password 를 입력합니다.

login succeeded 라는 구문이 뜨면 로그인 성공입니다.

도커 이미지를 올리기 전에 태그를 달아줍니다.

```jsx
sudo docker tag ok-node-test:0.0.1 wendyyi/ok-node-test:0.0.1
sudo docker image ls
```

명령어를 사용하여 이미지를 확인해보면 본인 username/ok-node-test 라는 repository 가 생긴것을 확인 할 수 있습니다. 이제 도커허브에 올릴 준비가 되었습니다.

```jsx
sudo docker push wendyyi/ok-node-test:0.0.1
```

이렇게 본인의 repository 로 push를 해줍니다

dockerhub 에 접속해서 myprofile 에 본인의 repository 를 확인하면 push 된것을 확인할수있습니다.

## 📣 AWS 환경에서 docker 이미지를 반영하기

터미널에서 ssh 를 이용하여 aws 개발 환경으로 접속한뒤 본인 repository 에 있는 것을 다운을 받아서 돌리기 위해서 docker login 을 진행합니다

```jsx
sudo docker login
sudo docker run -d -p 80:80 wendyyi/ok-node-test:0.0.1
```

이렇게 로그인을 해서 pull을 할수 있습니다.

```jsx
sudo docker ps
```

pull 받은것을 확인 할 수 있습니다.

이제 url 에 aws 환경 ip 를 확인하면 OK 가 나온것을 확인할수 있습니다!!

# 🥳


## 📣리액트란 무엇일까?

react 는 현재 협업에서 인기 잇는 웹/앱의 view를 개발할 수 있도록 하는 라이브러리이다.

보통 우리가 생각하는 어플리케이션(웹, 앱 혹은 데스크톱용 소프트웨어)을 만들기 위해서는 사용자가 조작하기 위한 UI, UI를 컨트롤 하기 위한 로직, 데이터를 처리하는 비즈니스 로직 등 3가지 부분으로 개발이 필요하다. 

이렇게 특정 부분을 나누어 개발하는 방법론을 MVC 패턴, MVVM패턴 이라고 하며, react.js 는 View 즉, 사용자가 조작하기 위한 UI를 만드는 것을 도와주는 라이브러리 이다.

 "컴포넌트" 라는 개념에 집중 되어있는 라이브러리이다. 컴포넌트를 간단하게 설명하자면, 데이터를 넣으면 우리가 지정한 유저 인터페이스를 조립해서 보여준다. 페이스북 개발자들이 라이브러리의 성능과 개발자 경험을 개선하기 위해 많은 연구를 한다. 생태계가 넓고, 사용하는 곳도 많다. HTTP 클라이언트, 라우터 , 심화적 상태 관리 등의 기능들은 내장되어 있지 않다. 따로 공식 라이브러리가 있는것도 아니여서 개발자가 원하는 스택을 맘대로 골라서 사용 할 수있다.

## 📣리액트의 특징

react.js 를 처음 배우면 react.js 의 특징으로 다음과 같은 말을 볼 수 있다.

1. react는 선언형이다.
2. react는 컴포넌트 기반으로 재사용성이 뛰어나다.
3. react는 virual DOM(가상돔)기반으로 가볍다.
4. react 컴포넌트는 state 와 props을 가진다.

여기에서 다음의 키워드를 얻을 수 있다. 선언형, 컴포넌트, 재사용성, 가상돔.

1. 선언형 Declarative 란

```jsx
소프트웨어 공학에서 자주 접하게 되는 개념은 패러다임이다. 즉, 프로그래밍을 어떻게 할 것인가
하는 생각에 대한 논의가 활발하게 이루어진다.
 이 중 리액트를 하면 자주 접할 수 있는 패러다임이 선언형 프로그래밍과 명령형 Imperative 
프로그래밍이다.
리액트는 선언형 성격에 맞게 컴포넌트(원하는 결과,뷰)를 얻기위해 <tag></tag>jsx문법을 통해
구현한다. 즉, jsx를 얻기 위한 알고리즘에 대한 구현을 하지 않는다.(예를들어,
document.createElement 나 혹은 해당 컴포넌트의 변경사항을 체크하는 알고리즘, 리-렌더링 여부에
대한 알고리즘을 구현하지 않는다.)
 이와 같은 선언형 특성은, 리액트를 사용할 때 화면 설계라는 초점에 맞춰서 개발할 수 있도록 해주므로,
다른 부분에 대한 고민을 최소화해주어 높은 생산성을 보장할 수 있도록 해준다.
```

2. 컴포넌트 및 재사용성

```jsx
리액트를 쓰는 지금 컴포넌트(Component)라는 개념을 통해 작성한 HTML,CSS를 간략하게
<Component/> 와 같은 식으로 쓸 수 있다.
 컴포넌트는 구현, 명세화, 패키지화, 그리고 배포될 수 있어야 한다.
 컴포넌트는 독립적인 단위의 소프트웨어 모듈을 말한다. 즉 소프트웨어를 독립적인 하나의 부품으로
만드는 방법이다. 리액트는 웹에서 쓰는 각 요소들을 컴포넌트로 만들 수 있게 해 기존의 UI를 다른
화면에서 다시 쓸 수 있도록 하는 장점(높은 재사용성)을 가진다
```

3. Virtual DOM(가상돔)

```jsx
가상돔을 이해하기 위해선 In-memory의 개념에 대해 알아두면 좋다. 웹브라우저와 자바스크립트를
동작시키기 위한 V8엔진도 소프트웨어이다. 즉, 이들이 실행되면 메모리(RAM)이 할당이 된다.
 가상돔은 이 메모리 단에서 컴포넌트에 대한 정보를 생성하고 비교하여 전체 DOM트리가
업데이트가 필요한 경우 이를 반영하는 방식을 말한다.
 만약, 실제 DOM 트리에서 변화가 바로바로 반영된다면 하나의 동작(입력값변화, 데이터 변화)마다
전체 DOM트리가 변경되어 브라우저 렌더링 과정(HTML 파싱, 렌더 ㅌ트리 배치, 렌더 트리 그리기
등의 과정)이 매번 일어나서 웹 브라우저의 동작에 많은 리소스가 들어가게 된다.
```

4. State 와 Props

```jsx
리액트는 내부적으로 State와 Props를 가진다. 이는, UI가 사용자의 동작에 따라 다른 UI나
Action이 필요하기 때문이다.
 리액트를 잘 다루기 위해서는 이런 State 에 대한 이해가 필요하다. 어떤 컴포넌트를 만들 때,
내부 컴포넌트에 어떤 State가 있을지, 페이지 전체에 어떤 State가 있는지 파악하고 개발을
진행하는 것이 좋다.
 리액트로 UI 개발을 한다면 State와 Props를 어떻게 구성할 것인지를 먼저 파악하고
개발하도록 하는것이 좋다.
```

## 📣SPA 란?

SPA 란 Single Page Application의 약자이다.

단일 페이지 어플리케이션(SPA)는 현재 웹개발의 트랜드이다.

기존 웹 서비스는 요청시마다 서버로부터 리소스들과 데이터를 해석하고 화면에 렌더링하는 방식이다. SPA 형태는 브라우저에 최초에 한번 페이지 전체를 로드하고, 이후부터는 특정 부분만 Ajax를 통해 데이터를 바인딩 하는 방식이다.

            전통적인 페이지 vs 단일 페이지 어플리케이션 비교

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/6f55d2d4-8002-405c-b093-969cf7cca167/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/6f55d2d4-8002-405c-b093-969cf7cca167/Untitled.png)

## 📣SPA 장점과 단점  

- 장점
    1. 손쉬운 운영 배포

        ⇒ 전통적인 웹 개발 방식과 달리 Client Side와 Server Side 에서 하는 역할에 대해 분리가 가능하며 배포가 기존 웹개발보다 쉽다

    2. 사용자 친화적

        ⇒사용자 측면에서 일정한 전체 페이지 새로 고침 혹은 웹사이트에서 정보를 얻기 위해 앞뒤      로 왔다갔다 하는 것은 과도한 네트워크 트래픽을 유도하고 편이성 마저 떨어진다.

    3. 서버 요청이 적음(REST API를 통한 데이터 송수신)

        ⇒ 필요한 부분의 데이터만 요청하기 때문에 서버 요청이 적다.

        초기 페이지로드 후에 SPA에서 네트워크를 통해 더이상 HTML이 전송되지 않는다.

        SPA가 실행되는 동안 데이터만 유선을 통해 전송이 되므로 HTML을 지속적으로 보내는 것보다 시간과 대역폭이 훨씬 적다.

- 단점
    1. 검색 엔진 최적화에는 어려움이 있습니다.

        ⇒ SPA는 서버 렌더링 방식이 아닌 js 기반의 비동기 모델이다.

        View를 생성하는데 js 가 필요하다. 하지만 대부분의 웹 크롤러 봇들은 js파일을 실행시키지 못한다. 따라서 클라이언트 렌더링 방식 페이지를 빈 페이지로인식하게 되어, 웹 크롤러들은 내용을 알 수 없고 제대로 된 데이터를 수집 할 수 없다.

        (웹크롤러는 스파이더 또는 검색 엔진 봇이라고도 하고, 전체 인터넷에서 콘텐츠를 다운로드하고 색인을 생성한다. 이러한 봇의 목표는 웹 상의 모든 웹페이가 무엇에 대한 것인지 파악하여 필요할 때 정보를 추출할 수 있도록 하는것이다. 웹 크롤러라고 부르는 것은 소프트웨어 프로그램을 통해 자동으로 웹사이트에 엑세스하여 데이터를 얻는 일을 기술 용어로 크롤링이라고 하기 때문)

    2. 초기 구동에 시간이 걸림

        ⇒ 웹 애플리케이션에 필요한 모든 정적 리소스를 최초에 한번 다운로드하기 때문에

## 📣 React 주요 개념

가장 단순하 React 예시는 다음과 같이 생겼습니다.

```jsx
ReactDOM.render(
	<h1>Hello, world!</h1>
	document.getElementById('root')
);
```

아래 변수 선언을 살펴봅시다.

```jsx
const element = <h1>Hello, world!</h1>
```

위에 태그 문법은 문자열도, HTML도 아닙니다.

JSX라고 하며 JavaScript를 확장한 문법입니다. JSX는 React "엘리먼트(element)"를 생성합니다.

### 🗨️JSX란?

React에서는 이벤트가 처리되는 방식, 시간에 따라 state 가 변하는 방식, 화면에 표기하기 위해 데이터가 준비되는 방식 등 렌더링 로직이 본질적으로 다른 UI 로직과 연결된다는 사실을 받아드립니다.

React는 별도의 파일에 마크업과 로직을 넣어 기술을 인위적으로 분리하는 대신, 둘 다 포함하는 "컴포넌트"라고 부르는 느슨하게 연결된 유닛으로 관심사를 분리합니다. 이후 섹션에서 다시 컴포넌트로 돌아오겠지만, JS에 마크업을 넣는 게 익숙해지지 않는다면 이 이야기가 확신을 줄 것입니다.

React는 JSX 사용이 필수가 아니지만, 대부분의 사람은 js코드 안에서 UI관련 작업을 할 때 시각적으로 더 도움이 된다고 생각합니다. 또한 React가 더욱 도움이 되는 에러 및 경고 메시지를 표시할 수 있게 해줍니다.

## 📣 React 설치하기

```jsx
npm install -g create-react-app
create-react-app my-app
```

- 새 프로젝트의 src/ 폴더에 있는 모든 파일들을 삭제해주세요.(폴더 안의 내용만 삭제하되 폴더는 삭제하면 안됨)

```jsx
cd my-app
sudo rm -f src/*
```

- [CSS 코드](https://codepen.io/gaearon/pen/oWWQNa?editors=0100)를 src/ 폴더에 index.css 파일로 추가해주세요.
- [JS 코드](https://codepen.io/gaearon/pen/oWWQNa?editors=0010)를 src/ 폴더에 index.js 파일로 추가해주세요.
- src/ 폴더에 있는 index.js 의 최상단에 아래 세 줄을 추가해주세요.

```jsx
import React from 'react';
import ReactDOM from 'react-dom';
import './index.css';
```

```jsx
🤚혹시 추가시 권한이 없어서 파일 생성이 안되면
sudo chmod 777 /home/myplanet/my-app/*
을 해주세요!    
```

- 자! 이제 npm start 명령어를 실행하고 [localhost:3000](http://localhost:3000) 을 확인해보세요!


## 📣 React 주요 개념

가장 단순하 React 예시는 다음과 같이 생겼습니다.

```jsx
ReactDOM.render(
	<h1>Hello, world!</h1>
	document.getElementById('root')
);
```

아래 변수 선언을 살펴봅시다.

```jsx
const element = <h1>Hello, world!</h1>
```

위에 태그 문법은 문자열도, HTML도 아닙니다.

JSX라고 하며 JavaScript를 확장한 문법입니다. JSX는 React "엘리먼트(element)"를 생성합니다.

### 📣JSX 란?

React에서는 이벤트가 처리되는 방식, 시간에 따라 state 가 변하는 방식, 화면에 표기하기 위해 데이터가 준비되는 방식 등 렌더링 로직이 본질적으로 다른 UI 로직과 연결된다는 사실을 받아드립니다.

React는 별도의 파일에 마크업과 로직을 넣어 기술을 인위적으로 분리하는 대신, 둘 다 포함하는 "컴포넌트"라고 부르는 느슨하게 연결된 유닛으로 관심사를 분리합니다. 이후 섹션에서 다시 컴포넌트로 돌아오겠지만, JS에 마크업을 넣는 게 익숙해지지 않는다면 이 이야기가 확신을 줄 것입니다.

React는 JSX 사용이 필수가 아니지만, 대부분의 사람은 js코드 안에서 UI관련 작업을 할 때 시각적으로 더 도움이 된다고 생각합니다. 또한 React가 더욱 도움이 되는 에러 및 경고 메시지를 표시할 수 있게 해줍니다.

## 📣 vscode - index.js

index.js 파일에 코드를 추가합니다.

```jsx
import React from 'react';
import ReactDOM from 'react-dom';
import './index.css';

class Square extends React.Component {
    state = {
      num : 0
    };

    change = () => {
      this.setState({
        num: this.state.num + 1,
      });
      //document.getElementById('a').textContent = 'aaaa';
    };
    
    render() {
        const status  = 'react! 버튼 클릭횟수';
        
      return (
        <div>
            <div><span>{status}</span></div>
            <div>
              {this.state.num}
              <button onClick={this.change}>Click Me!</button>
            </div>
        </div>
      );
    }
  }

  
  // ========================================
  
  ReactDOM.render(
    // <Game />,
    // <Board />,
    <Square />,
    document.getElementById('root')
  );
```

이렇게 코드를 넣은뒤에 terminal 에서

```jsx
sudo npm start
```

명령을 하고 Compiled successfully! 라고 뜨면 [localhost:3000](http://localhost:3000) 을 확인해주세요

그럼 버튼을 누를때 숫자가 (+) 되는 것을 확인 할수 있습니다.;

이제 docker-compose.yml 파일과 dockerfile 를 통해 도커 환경을 구성합니다.

docker-compose.yml 파일을 생성합니다

```jsx
version: '3.7'

services:

  countview_app:
    container_name: countview_app
    build:
      context: .
      dockerfile: dockerfile
    volumes:
      - '.:/app'
      - '/app/node_modules'
    ports:
      - '3000:3000'
    environment:
      - NODE_ENV=development
      - CHOKIDAR_USEPOLLING=true
```

위와 같이 코드를 넣어주세요. 마지막에 CHOKIDAR_USEPOLLING=true은 APP이 수정되었을 경우에 reload가 가능하도록 하는 설정입니다.




```jsx
import React,{ useState } from 'react';
import ReactDOM from 'react-dom';
import './index.css';

function Square(){

  const [number, setNumber] = useState(0);

  return(
    <div>
      <div>
        <h2>v: {number}</h2>
        <button onClick={() => {
          setNumber((v) => v + 1);
        }}>버튼</button>
      </div>
    </div>
  );
}

  
  ReactDOM.render(
    <Square />,
    document.getElementById('root')
  );
```

### 📣 ajax 란 무엇인가?

⇒ Ajax 는 javascript 의 라이브러리 중 하나이고 Asynchronous Javascript And Xml(비동기식 자바스크       립트와 xml)의 약자입니다. 브라우저가 가지고 있는 XMLHttpRequest 객체를 이용해서 전체 페이지를 새로 고치지 않고도 페이지의 일부만을 위한 데이터를 로드하는 기법이며, Ajax를 한마디로 정의하면 jsvascript를 사용한 비동기 통신, 클라이언트와 서버간에 XML 데이터를 주고받는 기술이라고 할 수 있습니다.

### 📣 Ajax 의 장점

1. 웹페이지의 속도 향상
2. 서버의 처리가 완료 될때까지 기다리지 않고 처리 가능하다.
3. 서버에서 Data만 전송하면 되므로 전체적은 코드양이 줄어든다.
4. 기존 웹에서는 불가능했던 다양한 UI를 가능하게 해준다.
