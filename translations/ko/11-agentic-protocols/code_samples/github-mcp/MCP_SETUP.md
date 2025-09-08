<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "c4be907703b836d1a1c360db20da4de9",
  "translation_date": "2025-08-30T14:59:53+00:00",
  "source_file": "11-agentic-protocols/code_samples/github-mcp/MCP_SETUP.md",
  "language_code": "ko"
}
-->
# MCP 서버 통합 가이드

## 사전 준비 사항
- Node.js 설치 (버전 14 이상)
- npm 패키지 관리자
- 필요한 종속성을 갖춘 Python 환경

## 설정 단계

1. **MCP 서버 패키지 설치**
   ```bash
   npm install -g @modelcontextprotocol/server-github
   ```

2. **MCP 서버 시작**
   ```bash
   npx @modelcontextprotocol/server-github
   ```  
   서버가 시작되면 연결 URL이 표시됩니다.

3. **연결 확인**
   - Chainlit 인터페이스에서 플러그 아이콘(🔌)을 찾으세요.
   - 플러그 아이콘 옆에 숫자 (1)가 나타나면 연결이 성공적으로 이루어진 것입니다.
   - 콘솔에 "GitHub plugin setup completed successfully"라는 메시지(추가 상태 라인 포함)가 표시됩니다.

## 문제 해결

### 일반적인 문제

1. **포트 충돌**
   ```bash
   Error: listen EADDRINUSE: address already in use
   ```  
   해결 방법: 포트를 변경하세요:
   ```bash
   npx @modelcontextprotocol/server-github --port 3001
   ```

2. **인증 문제**
   - GitHub 자격 증명이 올바르게 구성되었는지 확인하세요.
   - .env 파일에 필요한 토큰이 포함되어 있는지 확인하세요.
   - GitHub API 접근 권한을 확인하세요.

3. **연결 실패**
   - 서버가 예상 포트에서 실행 중인지 확인하세요.
   - 방화벽 설정을 확인하세요.
   - Python 환경에 필요한 패키지가 설치되어 있는지 확인하세요.

## 연결 확인

MCP 서버가 제대로 연결되었는지 확인하려면:
1. 콘솔에 "GitHub plugin setup completed successfully"라는 메시지가 표시됩니다.
2. 연결 로그에 "✓ MCP Connection Status: Active"가 표시됩니다.
3. GitHub 명령이 채팅 인터페이스에서 작동합니다.

## 환경 변수

.env 파일에 필요한 항목:
```
GITHUB_TOKEN=your_github_token
MCP_SERVER_PORT=3000  # Optional, default is 3000
```

## 연결 테스트

채팅에서 다음 테스트 메시지를 보내세요:
```
Show me the repositories for username: [GitHub Username]
```  
성공적인 응답은 저장소 정보를 표시합니다.

---

**면책 조항**:  
이 문서는 AI 번역 서비스 [Co-op Translator](https://github.com/Azure/co-op-translator)를 사용하여 번역되었습니다. 정확성을 위해 최선을 다하고 있지만, 자동 번역에는 오류나 부정확성이 포함될 수 있습니다. 원본 문서를 해당 언어로 작성된 상태에서 권위 있는 자료로 간주해야 합니다. 중요한 정보의 경우, 전문적인 인간 번역을 권장합니다. 이 번역 사용으로 인해 발생하는 오해나 잘못된 해석에 대해 책임을 지지 않습니다.