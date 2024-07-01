# -Csharp-Socket-Based-Network-Communication-Chat-Program
이 프로젝트는 C#으로 작성된 TCP 기반 클라이언트-서버 채팅 애플리케이션으로 구성되어 있습니다.
C# 소켓을 이용한 네트워크 통신 채팅 프로그램 README
개요
이 프로젝트는 C#으로 작성된 TCP 기반 클라이언트-서버 채팅 애플리케이션으로 구성되어 있습니다. 이 솔루션은 두 가지 주요 구성 요소를 포함합니다:

TCPClient - 사용자가 서버에 연결하고 채팅에 참여하는 클라이언트 애플리케이션입니다.
TCPServer - 클라이언트 연결을 처리하고 클라이언트 간 메시지 교환을 지원하는 서버 애플리케이션입니다.
프로젝트 구조
프로젝트 디렉토리는 다음과 같은 구조를 가집니다:

mathematica
코드 복사
Csharp_soket_chat_program/
│
├── TCPClient/
│   ├── TCPClient.sln
│   ├── TCPClient/
│   │   ├── App.config
│   │   ├── Form1.cs
│   │   ├── Form1.Designer.cs
│   │   ├── Form1.resx
│   │   ├── Program.cs
│   │   ├── TCPClient.csproj
│   │   ├── bin/
│   │   │   ├── Debug/
│   │   │   │   ├── TCPClient.exe
│   │   │   │   ├── TCPClient.exe.config
│   │   │   │   ├── TCPClient.pdb
│   │   ├── obj/
│   │       ├── Debug/
│   │           ├── .NETFramework,Version=v4.7.2.AssemblyAttributes.cs
│   │           ├── DesignTimeResolveAssemblyReferences.cache
│   │           ├── TCPClient.csproj.FileListAbsolute.txt
│   │           ├── TCPClient.csproj.GenerateResource.cache
│   │           ├── TCPClient.pdb
│
├── TCPServer/
│   ├── TCPServer.sln
│   ├── TCPServer/
│   │   ├── Form1.cs
│   │   ├── Form1.Designer.cs
│   │   ├── Form1.resx
│   │   ├── Program.cs
│   │   ├── TCPServer.csproj
│   │   ├── bin/
│   │   │   ├── Debug/
│   │   │       ├── TCPServer.exe
│   │   │       ├── TCPServer.exe.config
│   │   │       ├── TCPServer.pdb
│   │   ├── obj/
│   │       ├── Debug/
│   │           ├── .NETFramework,Version=v4.7.2.AssemblyAttributes.cs
│   │           ├── DesignTimeResolveAssemblyReferences.cache
│   │           ├── TCPServer.csproj.FileListAbsolute.txt
│   │           ├── TCPServer.csproj.GenerateResource.cache
│   │           ├── TCPServer.pdb
│   ├── Properties/
│       ├── AssemblyInfo.cs
│       ├── Resources.Designer.cs
│       ├── Resources.resx
│       ├── Settings.Designer.cs
│       ├── Settings.settings
사전 요구 사항
.NET Framework 4.7.2 이상
Visual Studio 2019 이상
프로젝트 설정
저장소 클론:
프로젝트 파일을 다운로드하고 원하는 위치에 압축을 해제합니다.

솔루션 열기:
Visual Studio에서 TCPClient.sln 및 TCPServer.sln 파일을 엽니다.

프로젝트 빌드:
TCPClient와 TCPServer 프로젝트를 빌드하여 필요한 패키지를 복원하고 소스 코드를 컴파일합니다.

애플리케이션 실행
서버 시작:

Visual Studio에서 TCPServer 프로젝트를 엽니다.
프로젝트를 실행합니다(F5 또는 Ctrl+F5).
서버 애플리케이션이 시작되며 클라이언트 연결을 대기합니다.
클라이언트 시작:

Visual Studio에서 TCPClient 프로젝트를 엽니다.
프로젝트를 실행합니다(F5 또는 Ctrl+F5).
서버 IP 주소와 포트 번호를 입력하여 서버에 연결합니다.
연결되면 메시지를 주고 받을 수 있습니다.
주요 구성 요소
TCPClient:

Form1.cs: UI 및 사용자 상호작용을 처리합니다.
Program.cs: 클라이언트 애플리케이션의 진입점입니다.
App.config: 클라이언트 구성 파일입니다.
TCPServer:

Form1.cs: 서버 측 UI 및 클라이언트 관리를 처리합니다.
Program.cs: 서버 애플리케이션의 진입점입니다.
AssemblyInfo.cs: 서버 어셈블리에 대한 메타데이터입니다.
기능
기본적인 TCP 소켓 통신
다중 클라이언트 지원(서버에서 처리)
Windows Forms를 이용한 간단한 GUI
연결된 클라이언트 간 실시간 메시징
향후 개선 사항
안전한 통신을 위한 메시지 암호화 구현
사용자 인증 추가
사용자 경험 향상을 위한 UI 디자인 개선
서버 및 클라이언트 활동 로그 기능 추가
문제 해결
클라이언트를 시작하기 전에 서버가 실행 중인지 확인합니다.
지정된 포트에서 TCP 연결을 허용하도록 방화벽 설정을 확인합니다.
클라이언트 애플리케이션에 올바른 서버 IP 주소와 포트 번호가 입력되었는지 확인합니다.
