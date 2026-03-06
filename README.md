# Super Star Trek

> 🇬🇧 English documentation is available [below](#english).

クラシックなテキストゲーム **Super Star Trek** を，ブラウザで遊べるGUIアプリとして実装したものです．

🎮 **[Play Now](https://your-username.github.io/your-repo/)**

---

## ゲームについて

**Super Star Trek** は，宇宙艦エンタープライズの艦長となって銀河を舞台に戦略的な宇宙戦を繰り広げる，ターン制のストラテジーゲームです．

銀河は 8×8 のクアドラントに分かれており，各クアドラントはさらに 8×8 のセクターに区切られています．プレイヤーはワープ航法で銀河を渡り歩きながら，クリンゴン艦を発見して撃破していきます．エネルギー・光子魚雷・シールド・各システムのダメージ状態を管理しながら，**任務期限（スターデート）までに全クリンゴン艦を殲滅**することが目標です．

宇宙基地に立ち寄ればエネルギーと魚雷を補給し，破損したシステムを修理できます．クリンゴンはプレイヤーの行動に反応して攻撃してくるため，シールド管理と艦の消耗をいかに抑えるかが鍵となります．

オリジナルは1970年代に BASIC で書かれたテキストゲームで，そのソースコードをもとに GUI として再実装したものです：

- [coding-horror/basic-computer-games](https://github.com/coding-horror/basic-computer-games/tree/main/84_Super_Star_Trek)

---

## 遊び方

### 目標

銀河（8×8クアドラント）に散らばる**クリンゴン艦**をすべて撃破し，任務期限内に帰還せよ．

### コマンド

| コマンド | 説明 |
|----------|------|
| **NAV** | ワープ航法．円が表示されるのでクリックしてコースを指定し，ワープ係数を入力して移動する |
| **SRS** | 近距離センサースキャン．現在のセクター内の状況を表示 |
| **LRS** | 長距離センサースキャン．隣接クアドラントの概要を表示 |
| **PHA** | フェーザー砲発射．投入エネルギー量を指定する |
| **TOR** | 光子魚雷発射．円が表示されるのでクリックしてコースを指定する（残数に注意）|
| **SHE** | シールドにエネルギーを転送する |
| **DAM** | ダメージコントロールレポートを表示 |
| **COM** | 艦載コンピュータ（銀河マップ，ナビ計算など） |
| **XXX** | ゲーム終了 |

### コース指定

NAV・TORでは円が表示されます．円上をクリックして方向（コース）を指定してください．NAVはその後ワープ係数の入力が必要です．

### 操作のヒント

- NAV・TORでは円が表示されます．円上をクリックしてコースを指定してください
- 宇宙基地に隣接してドッキングするとエネルギー・魚雷・修理が全回復します
- クリンゴンはターン毎に攻撃してきます．シールドを忘れずに

### 言語

画面右上の 🌐 ボタンで日本語⇔英語を切り替えられます（ゲームはリスタートされます）．

---

## ファイル構成

```
index.html   # ゲーム本体（HTML / CSS / JavaScript をすべて含む単一ファイル）
README.md    # このファイル
```

---

## ライセンス

オリジナルゲームは [coding-horror/basic-computer-games](https://github.com/coding-horror/basic-computer-games) の MIT ライセンスに準拠します．

---

## English

> 🇯🇵 日本語のドキュメントは[上](#super-star-trek)にあります。

A browser-based GUI implementation of the classic BASIC game **Super Star Trek**.

🎮 **[Play Now](https://your-username.github.io/your-repo/)**

### About the Game

**Super Star Trek** is a turn-based strategy game in which you take command of the starship Enterprise and wage a tactical space battle across the galaxy.

The galaxy is divided into an 8×8 grid of quadrants, each further subdivided into an 8×8 grid of sectors. You navigate by warp drive, hunt down Klingon warships, and destroy them — all before the stardate deadline expires. Managing your energy, photon torpedoes, shields, and system damage is the key to survival.

Starbases let you resupply and repair. Klingons react to your moves and fire back, so how well you protect your ship and conserve resources decides the outcome.

The original is a text-based BASIC game from the 1970s. This project re-implements it as a browser GUI:

- [coding-horror/basic-computer-games](https://github.com/coding-horror/basic-computer-games/tree/main/84_Super_Star_Trek)

### How to Play

#### Objective

Destroy all **Klingon ships** spread across the galaxy (8×8 quadrants) before the stardate deadline.

#### Commands

| Command | Description |
|---------|-------------|
| **NAV** | Warp navigation. A circle appears — click to set course, then enter warp factor |
| **SRS** | Short-range sensor scan — shows current sector |
| **LRS** | Long-range sensor scan — shows adjacent quadrants |
| **PHA** | Fire phasers. Enter energy units to fire |
| **TOR** | Fire photon torpedo. A circle appears — click to set course; limited supply |
| **SHE** | Transfer energy to shields |
| **DAM** | Damage control report |
| **COM** | Ship's computer (galaxy map, navigation calculator, etc.) |
| **XXX** | Resign / end game |

#### Course Selection

For NAV and TOR, a circle appears on screen. Click anywhere on the circle to set your course direction. NAV then prompts for a warp factor.

#### Tips

- Dock at a starbase (move adjacent to one) to fully replenish energy, torpedoes, and repairs
- Klingons fire back every turn — keep your shields up!

#### Language

Use the 🌐 button in the top-right corner to switch between Japanese and English (the game will restart).

### File Structure

```
index.html   # Complete game — HTML, CSS, and JavaScript in a single file
README.md    # This file
```

### License

Based on the original game from [coding-horror/basic-computer-games](https://github.com/coding-horror/basic-computer-games), MIT License.
