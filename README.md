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

## Official Lesson Code Reference

- Official repo: [CryptozombiesHQ/cryptozombies-lesson-code](https://github.com/CryptozombiesHQ/cryptozombies-lesson-code)
- Local reference: `references/cryptozombies-lesson-code`
- Lesson 1 source: `references/cryptozombies-lesson-code/lesson-1`
- Lesson 2 source: `references/cryptozombies-lesson-code/lesson-2`
- GitHub Lesson 1 source: [lesson-1](https://github.com/CryptozombiesHQ/cryptozombies-lesson-code/tree/master/lesson-1)
- GitHub Lesson 2 source: [lesson-2](https://github.com/CryptozombiesHQ/cryptozombies-lesson-code/tree/master/lesson-2)

The official lesson code is included as a Git submodule for study reference only. These samples are not production-ready, and the original repository is licensed under GPL-3.0.

## Reflection

CryptoZombies Lesson 1을 통해 Solidity로 데이터를 정의하고 함수를 통해 상태를 변경하는 기본 흐름을 익혔습니다.

좀비 생성 로직을 따라가면서 `contract`, `struct`, `array`, `function`이 스마트 컨트랙트 안에서 어떻게 연결되는지 확인했습니다.

CryptoZombies Lesson 2에서는 좀비 소유권을 `mapping`으로 관리하고, `msg.sender`와 `require`를 통해 호출자의 권한을 제한하는 패턴을 실습했습니다.

또한 `import`, 상속, 외부 컨트랙트 인터페이스를 사용해 CryptoKitties 컨트랙트의 데이터를 읽고, 기존 좀비 DNA와 섞어 새로운 좀비를 만드는 흐름을 정리했습니다.

## Next Steps

- Start CryptoZombies Lesson 3 and keep adding progress notes.
- Build a simple ERC20 staking vault with tests.
- Build a mini AMM inspired by Uniswap v2.
- Study DeFi security challenges and write short vulnerability notes.

## Portfolio Direction

This repository is the starting point of my Web3 developer portfolio. Future project repositories will focus on production-style Solidity development, including:

- `staking-vault`
- `mini-amm`
- `mini-lending-protocol`
- `defi-security-writeups`
