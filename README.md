# Web3 Learning Log

Solidity와 DeFi 개발자가 되기 위한 학습 기록입니다.

이 저장소는 완성된 서비스보다 학습 과정, 실습 결과, 배운 개념, 다음 목표를 꾸준히 남기기 위한 포트폴리오입니다.

## CryptoZombies Progress

### Lesson 1: Zombie Factory

- Result: BLOX
- Share: [BLOX Zombie](https://share.cryptozombies.io/ko/lesson/1/share/BLOX?id=Y3p8NjczNTA4)
- Learned:
  - Solidity contract structure
  - State variables
  - Structs and arrays
  - Public functions
  - Basic zombie creation logic

### Lesson 2: Zombies Attack Their Victims

- Result: BLOX reached level 2
- Share: [BLOX Lesson 2 Zombie](https://share.cryptozombies.io/ko/lesson/2/share/BLOX?id=Y3p8NjczNTA4)
- Added: unnamed cat-zombie hunter
- Learned:
  - Contract inheritance and imports
  - `mapping` for zombie ownership
  - `msg.sender` for caller-based permissions
  - `require` for access control
  - `storage` references for updating structs
  - External contract interfaces for CryptoKitties
  - DNA mixing logic for zombie feeding

### Lesson 3: Advanced Solidity Concepts

- Result: BLOX reached level 3, SATA reached level 2
- Share: [BLOX Lesson 3 Zombie Army](https://share.cryptozombies.io/ko/lesson/3/share/BLOX?id=Y3p8NjczNTA4)
- Updated: renamed the former NoName kitty zombie to SATA
- Learned:
  - `Ownable` ownership pattern
  - `modifier` usage for reusable access checks
  - `onlyOwner` for protected admin functions
  - Gas and storage optimization basics
  - Zombie levels and cooldown timers
  - Level-gated `changeName` and `changeDna` functions
  - Returning owner-specific zombie armies with view functions

### Lesson 4: Zombie Battle System

- Result: BLOX reached level 4
- Share: [BLOX Lesson 4 Zombie Army](https://share.cryptozombies.io/ko/lesson/4/share/BLOX?id=WyJjenw2NzM1MDgiLDEsMTRd)
- Added: new level 1 zombie from battle rewards
- Learned:
  - `payable` functions and Ether-based level-up fees
  - Contract balance withdrawal with `onlyOwner`
  - Reusable `ownerOf` modifier for zombie permissions
  - Internal cooldown checks before feeding and battling
  - Pseudo-random battle outcomes with `keccak256`
  - `winCount` and `lossCount` battle statistics
  - Reward flow for leveling up and creating a new zombie after victory

### Lesson 5: ERC721 and Crypto-Collectibles

- Result: received level 10 H4XF13LD MORRIS zombie
- Share: [H4XF13LD MORRIS Zombie Army](https://share.cryptozombies.io/ko/lesson/5/share/H4XF13LD_MORRIS_💯💯😎💯💯?id=Y3p8NjczNTA4)
- Army size: 4 zombies
- Learned:
  - Tokens and the ERC721 NFT standard
  - `balanceOf`, `ownerOf`, `approve`, and `transferFrom`
  - `Transfer` and `Approval` events for off-chain tracking
  - Approval mapping for delegated zombie transfers
  - Solidity libraries with `using SafeMath for uint256`
  - Overflow and underflow protection with SafeMath
  - Code comments and NatSpec documentation basics

## Official Lesson Code Reference

- Official repo: [CryptozombiesHQ/cryptozombies-lesson-code](https://github.com/CryptozombiesHQ/cryptozombies-lesson-code)
- Local reference: `references/cryptozombies-lesson-code`
- Lesson 1 source: `references/cryptozombies-lesson-code/lesson-1`
- Lesson 2 source: `references/cryptozombies-lesson-code/lesson-2`
- Lesson 3 source: `references/cryptozombies-lesson-code/lesson-3`
- Lesson 4 source: `references/cryptozombies-lesson-code/lesson-4`
- Lesson 5 source: `references/cryptozombies-lesson-code/lesson-5`
- GitHub Lesson 1 source: [lesson-1](https://github.com/CryptozombiesHQ/cryptozombies-lesson-code/tree/master/lesson-1)
- GitHub Lesson 2 source: [lesson-2](https://github.com/CryptozombiesHQ/cryptozombies-lesson-code/tree/master/lesson-2)
- GitHub Lesson 3 source: [lesson-3](https://github.com/CryptozombiesHQ/cryptozombies-lesson-code/tree/master/lesson-3)
- GitHub Lesson 4 source: [lesson-4](https://github.com/CryptozombiesHQ/cryptozombies-lesson-code/tree/master/lesson-4)
- GitHub Lesson 5 source: [lesson-5](https://github.com/CryptozombiesHQ/cryptozombies-lesson-code/tree/master/lesson-5)

The official lesson code is included as a Git submodule for study reference only. These samples are not production-ready, and the original repository is licensed under GPL-3.0.

## Reflection

CryptoZombies Lesson 1을 통해 Solidity로 데이터를 정의하고 함수를 통해 상태를 변경하는 기본 흐름을 익혔습니다.

좀비 생성 로직을 따라가면서 `contract`, `struct`, `array`, `function`이 스마트 컨트랙트 안에서 어떻게 연결되는지 확인했습니다.

CryptoZombies Lesson 2에서는 좀비 소유권을 `mapping`으로 관리하고, `msg.sender`와 `require`를 통해 호출자의 권한을 제한하는 패턴을 실습했습니다.

또한 `import`, 상속, 외부 컨트랙트 인터페이스를 사용해 CryptoKitties 컨트랙트의 데이터를 읽고, 기존 좀비 DNA와 섞어 새로운 좀비를 만드는 흐름을 정리했습니다.

CryptoZombies Lesson 3에서는 `Ownable`과 `modifier`를 통해 관리자 권한을 분리하고, 레벨과 쿨다운을 추가해 게임 로직을 더 안전하게 확장하는 방법을 배웠습니다.

특히 `onlyOwner`로 외부 컨트랙트 주소 변경 함수를 보호하고, `view` 함수로 사용자의 좀비 군대만 반환하는 패턴을 실습했습니다.

CryptoZombies Lesson 4에서는 `payable` 함수로 이더를 받는 레벨업 기능을 만들고, `withdraw`와 `setLevelUpFee`를 `onlyOwner`로 보호하는 운영 패턴을 배웠습니다.

전투 로직에서는 소유권 검증, 쿨다운 확인, 의사 난수 생성, 승패 기록, 승리 보상으로 새 좀비를 만드는 흐름을 하나의 게임 루프로 연결했습니다.

CryptoZombies Lesson 5에서는 좀비를 ERC721 스타일의 거래 가능한 토큰으로 다루기 위해 `balanceOf`, `ownerOf`, `approve`, `transferFrom` 흐름을 구현했습니다.

또한 `Transfer`와 `Approval` 이벤트가 외부 앱과 마켓플레이스에서 NFT 이동을 추적하는 표준 신호라는 점을 확인했고, `SafeMath` 라이브러리로 산술 연산을 더 안전하게 만드는 패턴을 익혔습니다.

## Next Steps

- Start CryptoZombies Lesson 6 and keep adding progress notes.
- Build a simple ERC20 staking vault with tests.
- Build a mini AMM inspired by Uniswap v2.
- Study DeFi security challenges and write short vulnerability notes.

## Portfolio Direction

This repository is the starting point of my Web3 developer portfolio. Future project repositories will focus on production-style Solidity development, including:

- `staking-vault`
- `mini-amm`
- `mini-lending-protocol`
- `defi-security-writeups`
