# 포트폴리오 10 — 문서화 · 온보딩

ADR·온보딩 체크리스트로 팀 지식을 코드처럼 관리

## 시리즈

- [01 — 보안관제·서비스·서버 운영](https://github.com/yunsunghun/portfolio-01-security-ops) (선행 레포)
- 본 저장소는 **10**번째 포트폴리오입니다.

## 빠른 탐색

- 기획: [docs/00-PORTFOLIO-BRIEF.md](docs/00-PORTFOLIO-BRIEF.md)
- GitHub Actions 활성화: [README 하단](#github-actions)

## GitHub Actions

`docs/reference-github-actions-ci.yml` 내용을 `.github/workflows/ci.yml` 로 복사한 뒤 커밋합니다.  
토큰에 `workflow` 권한이 필요합니다.

```bash
gh auth refresh -h github.com -s workflow
mkdir -p .github/workflows
cp docs/reference-github-actions-ci.yml .github/workflows/ci.yml
git add .github/workflows/ci.yml && git commit -m "ci: GitHub Actions 추가" && git push
```

## 라이선스

[LICENSE](LICENSE) (MIT) · [SECURITY.md](SECURITY.md)
