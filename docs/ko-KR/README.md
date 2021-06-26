---
home: true
heroImage: /logo.svg
heroText: null
tagline: 어떤 쉘에서도 쓸 수 있는 작고 극도로 빠르고 무한 변형이 가능한 프롬프트!
actionText: Get Started →
actionLink: ./guide/
features:
  - title: 호환성을 우선합니다
    details: 대부분의 운영체제에서, 대부분의 쉘에서 동작합니다. 모든 곳에서 쓰세요!
  - title: 러스트로 만들어졌습니다
    details: 러스트의 안정성과 동급 최고의 성능을 제공합니다. 최선의 빠르고 믿을 수 있는 프롬프트를 만들어 보세요.
  - title: 얼마든지 변형할 수 있습니다
    details: 모든 사소한 부분까지 당신의 입맛에 따라 바꿀 수 있습니다. 최소의 프롬프트를 만들거나 최대의 정보를 제공하는 프롬프트를 만들거나, 이 모든 것은 당신의 선택입니다.
footer: ISC Licensed | Copyright © 2019-present Starship Contributors

# Used for the description meta tag, for SEO
metaTitle: "Starship: Cross-Shell Prompt"
description: Starship은 어떤 쉘에서도 쓸 수 있는 작고 극도로 빠르고 최대로 변형할 수 있는 프롬프트입니다! 멋지고 최소한으로도 당신이 필요로하는 정보를 보여줍니다. Bash, ZSH, Ion, PowerShell에서도 빠르게 설치하여 사용할 수 있습니다.
---

<div class="center">
  <video class="demo-video" muted autoplay loop playsinline>
    <source src="/demo.webm" type="video/webm">
    <source src="/demo.mp4" type="video/mp4">
  </video>
</div>

### 빠른 설치

1. **starship** 바이너리 파일로 설치하기:

   #### 최신 버전 설치하기

   쉘로 설치하기:

   ```sh
   curl -fsSL https://starship.rs/install.sh | bash
   ```

   #### 패키지 메니저로 설치하기:

   [Homebrew](https://brew.sh/)로 설치하기:

   ```sh
   brew install starship
   ```

   [Scoop](https://scoop.sh)로 설치하기:

   ```powershell
   scoop install starship
   ```

1. 쉘 설정 파일에 초기화(init) 스크립트 넣기:

   #### Bash

   `~/.bashrc` 파일 마지막에 다음을 추가합니다:

   ```sh
   # ~/.bashrc

   eval "$(starship init bash)"
   ```

   #### Fish

    `~/.config/fish/config.fish` 파일 마지막에 다음을 추가합니다:

   ```sh
   # ~/.config/fish/config.fish

   starship init fish | source
   ```

   #### Zsh

   `~/.zshrc` 파일 마지막에 다음을 추가합니다:

   ```sh
   # ~/.zshrc

   eval "$(starship init zsh)"
   ```

   #### Powershell

   `Microsoft.PowerShell_profile.ps1` 파일 마지막에 다음을 추가합니다. 파워쉘에서 `$PROFILE` 변수에서 파일의 위치를 확인할 수 있습니다. 윈도우에서는 보통   `~\Documents\PowerShell\Microsoft.PowerShell_profile.ps1`이고 *닉스 계열은 `~/.config/powershell/Microsoft.PowerShell_profile.ps1`에 위치합니다.

   ```sh
   Invoke-Expression (&starship init powershell)
   ```

   #### Ion

   `~/.config/ion/initrc` 파일 마지막에 다음을 추가합니다:

   ```sh
   # ~/.config/ion/initrc

   eval $(starship init ion)
   ```
