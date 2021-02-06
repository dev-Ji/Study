# TIL


## 📣notion  이용방법

(notion 은 노트,일정,업무,데이터,프로젝트 등을 효율적으로 생성하고 관리할 수 있는 All-in-one 생상성 도구이자 협업 툴입니다.)

- 워크스페이스 섹션의 페이지들은 전체 팀이 할 수 있습니다.
- 개인페이지 섹션의 페이지들은 개인(본인)만 확인 할 수 있습니다.
- 개인페이지 섹션의 페이지 추가를 하려면 해당 섹션 페이지 옆에 (+) 버튼으로 추가 할 수 있습니다.
- 글 작성시, "/"를 누르면 명령어를 입력 할 수 있습니다.(토글 목록, 제목, 리스트, 이모지, ... 등등)
- 공유된 페이지 섹션에 있는 페이지는 초대나 권한을 받아야만 확인 할 수 있습니다.
- 공유된 페이지 중 Developers - 일반, Tech. 하위 메뉴들은 모두 중요하기 때문에 꼭 확인을 해야합니다.
- 일반 하위 메뉴 중 인프런 강의페이지를 보면 시청 할 수 있는 동영상 강의 목록이 뜹니다.(이용 원할시, 문성현 CTO님께 계정 요청)
- 해당글이나 문장에 댓글을 남기고 싶을때는 해당 문장 더블클릭 후 댓글 누르면 댓글을 남길 수 있습니다.
- 댓글 작성시 "@"를 누르면 멘션을 추가 할 수 있습니다.
- "ctrl+p" 누르면 검색을 할 수 있는데 "New challengers guideline"을 검색하면 마이플래닛의 가이드 라인을 확인 할 수 있습니다.
- 워크스페이스 섹션 중 프로젝트 하위에 일정을 클릭하면 일정을 확인 할 수 있습니다. 최근에는 프로젝트 일정은 Jira를 이용하여 관리합니다.

## 📣Slack 이용방법

(Slack 은 채널 기반 메시징 플랫폼입니다. 워크스페이스는 채널로 구성되어 있고 팀 멤버가 서로 커뮤니케이션하고 협업 할 수 있는 공간입니다.)

- 채널 섹션에 여러페이지 중 앞쪽에 자물쇠 표시가 있는 페이지는 초대를 받거나 권한을 확인 받아야 이용 할 수 있습니다.
- 다이렉트 메세지 섹션은 메세지를 보낼 수 있는 회원들을 확인 할 수 있습니다. 메세지를 보내기 위해서 해당 멤버를 클릭하면 해당멤버에게 메세지를 전송 할 수 있습니다.
- 대화방(개발)에서 "@here" 을 입력 후 메세지를 전송하게 되면 채널의 모든 온라인 멤버에게 알림이 뜹니다.
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
- 프로젝트 3개중에 개인 프로젝트나 과제프로젝트는 myplanet 에 이슈 등록 하면 됩니다.

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
