---
layout: default
title: 1. Omega
parent: Lv 90. TOP
grand_parent: Ultimates
permalink: /ultimates/top/01_omega/
---

# Omega

Omega的第一個型態被玩家稱為「蟑螂」, 這是整個戰鬥中陪伴玩家最久的一個型態。

---

## 循環程序

每位玩家會拿到一個數字debuff，分別是1、2、3和4，每種數字共會有兩名玩家拿到。

- **數字debuffs** 代表玩家需要踩塔的順序（1 > 2 > 3 > 4）。
- **接線** 需要兩名玩家接線遠離塔 (3 > 4 > 1 > 2)

當線爆炸的時候會產生一個大範圍Aoe， 給玩家一個2層毀滅與最大HP下降至1%的debuff。

HP的懲罰會在兩輪之後消失（治療需要照顧拿到3和4debuffs的玩家）。
<table>
  <tr>
    <td width="50%">
      <p>右圖是有可能生成塔的8個點.</p>
      <p>2個塔會同時生成， 並呈現90度或180度。</p>
      <p>每個塔生成位置不連續出現。</p>
      <p>我們使用以下的優先級來決定誰要去哪個塔／線:</p>
      <ul>
        <li><b>從西北開始順時針:</b> H1 MT ST D1 D2 D3 D4 H2</li>
      </ul>
    </td>
    <td><img src="https://tuufless.github.io/FFXIV-Elemental-Raid-Macros/assets/images/ultimates/top/01/program_loop_01.jpg"></td>
  </tr>
  <tr>
    <td>
      <p><b>1.</b> 第1輪塔生成</p>
      <ul>
        <li><b>3s:</b> 3號站在人群前面接線</li>
        <li><b>其餘玩家:</b> 集合在一起讓線更好接（別偷跑）</li>
      </ul>
    </td>
    <td><img src="https://tuufless.github.io/FFXIV-Elemental-Raid-Macros/assets/images/ultimates/top/01/program_loop_02.jpg"></td>
  </tr>
  <tr>
    <td>
      <p><b>1.</b>處理第1輪塔／線</p>
      <ul>
        <li><b>1號:</b> 踩塔。</li>
        <li><b>3號:</b> 接線。</li>
      </ul>
    </td>
    <td><img src="https://tuufless.github.io/FFXIV-Elemental-Raid-Macros/assets/images/ultimates/top/01/program_loop_03.jpg"></td>
  </tr>
  <tr>
    <td>
      <p><b>2.</b> 處理第2輪塔／線</p>
      <ul>
        <li><b>2號:</b> 踩塔。</li>
        <li><b>4號:</b> 接線。</li>
      </ul>
    </td>
    <td><img src="https://tuufless.github.io/FFXIV-Elemental-Raid-Macros/assets/images/ultimates/top/01/program_loop_04.jpg"></td>
  </tr>
  <tr>
    <td>
      <p><b>3.</b> 處理第3輪塔／線</p>
      <ul>
        <li><b>3號:</b> 踩塔。</li>
        <li><b>1號:</b> 接線。</li>
      </ul>
      <p>上一輪處理完畢後3號玩家的HP debuff消失，需要治療才能夠吃下塔的傷害。</p>
    </td>
    <td><img src="https://tuufless.github.io/FFXIV-Elemental-Raid-Macros/assets/images/ultimates/top/01/program_loop_05.jpg"></td>
  </tr>
  <tr>
    <td>
      <p><b>4.</b> 處理第4輪塔／線</p>
      <ul>
        <li><b>4號:</b> 踩塔</li>
        <li><b>2號:</b> 接線</li>
      </ul>
      <p>上一輪處理完畢後4號玩家的HP debuff消失，需要治療才能夠吃下塔的傷害。</p>
    </td>
    <td><img src="https://tuufless.github.io/FFXIV-Elemental-Raid-Macros/assets/images/ultimates/top/01/program_loop_06.jpg "></td>
  </tr>
</table>

在第4輪塔線處理完畢HP debuff也消失後，將玩家們的血量補滿，準備處理下個機制。

---

## 全能之主

參考 **HaruGlory** 的全能之主處理方式，將分攤波動炮放在後面，單點導彈放在前面。

<table>
  <tr>
    <td width="50%">
      <p><b>1.</b> 坦克將Omega面相拉北。</p>
      <p>其餘的人留在場中，準備調整（如果需要）。</p>
    </td>
    <td><img src="https://tuufless.github.io/FFXIV-Elemental-Raid-Macros/assets/images/ultimates/top/01/pantokrator_01.jpg"></td>
  </tr>
  <tr>
    <td>
      <p><b>2.</b> 隊伍會再次被上一輪1、2、3和4的數字debuffs。</p>
      <p>將隊伍拆成兩組，一組以北西為初始點, 另一組以南東為初始點:</p>
      <p>我們需要將隊伍以下列規範拆成兩組:</p>
      <ul>
        <li>組內需要1、2、3、4各1名。</li>
        <li>2組需要各1名治療。</li>
      </ul>
      <p>因此，我們參考以下優先級進行分組:</p>
      <ul>
        <li><b>北西:</b> H1 MT ST D1 D2 D3 D4 H2 <b>:南東</b></li>
      </ul>
    </td>
    <td><img src="https://tuufless.github.io/FFXIV-Elemental-Raid-Macros/assets/images/ultimates/top/01/pantokrator_03.jpg"></td>
  </tr>
</table>

第1組披薩出現，如果披薩覆蓋到了北西和南東， 轉 **順時針** 到旁邊的安全區。

以下是各種初始點（只有在第2與第3種情況需要順時針）。

<table>
  <tr>
    <td><img src="https://tuufless.github.io/FFXIV-Elemental-Raid-Macros/assets/images/ultimates/top/01/pantokrator_02a.jpg"></td>
    <td><img src="https://tuufless.github.io/FFXIV-Elemental-Raid-Macros/assets/images/ultimates/top/01/pantokrator_02a.jpg"></td>
    <td><img src="https://tuufless.github.io/FFXIV-Elemental-Raid-Macros/assets/images/ultimates/top/01/pantokrator_02c.jpg"></td>
    <td><img src="https://tuufless.github.io/FFXIV-Elemental-Raid-Macros/assets/images/ultimates/top/01/pantokrator_02d.jpg"></td>
  </tr>
</table>

<table>
  <tr>
    <td>
      <p>全能之主中的移動路徑:</p>
      <ol>
        <li>分攤炮判定。</li>
        <li>每個人向前移動離開預兆。</li>
      </ol>
      <p>每個人持續走停走停，下一個需要放單點導彈的玩家遠離人群:</p>
      <ol start="3">
        <li>在場中引導1次預兆</li>
        <li>將下個預兆引導至最遠的披薩旁（下輪的單點及分攤即將判定）.</li>
        <li>在外面或追著披薩再放一圈（以不妨礙到人群為主）。</li>
        <li>重新回到人群，在判定後還會有多1個預兆，也可以引導完後再回人群。</li>
      </ol>
    </td>
    <td><img src="https://tuufless.github.io/FFXIV-Elemental-Raid-Macros/assets/images/ultimates/top/01/pantokrator_movement.jpg"></td>
  </tr>
</table>

合在一起後看起來像這樣:
<img src="https://tuufless.github.io/FFXIV-Elemental-Raid-Macros/assets/images/ultimates/top/01/pantokrator.gif">
*(來源: Aqua Glacies)*

### 分攤波動炮 和 單點導彈

<table>
  <tr>
    <td width="50%">
      <p><b>6.</b> 數字debuffs與第1輪披薩出現。</p>
      <p>將隊伍拆成兩組，人群移動到安全區的中央等披薩燒過來</p>
      <ul>
        <li><b>1號:</b> 靠場中等待</li>
      </ul>
    </td>
    <td><img src="https://tuufless.github.io/FFXIV-Elemental-Raid-Macros/assets/images/ultimates/top/01/pantokrator_03.jpg"></td>
  </tr>
  <tr>
    <td>
      <p><b>7.</b> 披薩開始旋轉。</p>
      <p>1號追著最遠的披薩移動。</p>
      <p>其餘的玩家調整位置讓預兆正好落在轉過來的披薩上。</p>
    </td>
    <td><img src="https://tuufless.github.io/FFXIV-Elemental-Raid-Macros/assets/images/ultimates/top/01/pantokrator_04.jpg"></td>
  </tr>
  <tr>
    <td>
      <p><b>8.</b> 第3輪披薩</p>
      <p>第1組預兆出現在玩家們的腳下</p>
      <ul>
        <li><b>1號:</b> 引導你的預兆後移動。</li>
      </ul>
    </td>
    <td><img src="https://tuufless.github.io/FFXIV-Elemental-Raid-Macros/assets/images/ultimates/top/01/pantokrator_05.jpg"></td>
  </tr>
  <tr>
    <td>
      <p><b>9.</b> 第2組預兆（第1次分攤單點判定後）</p>
      <ul>
        <li><b>1秒:</b> 在遠披薩側吃單點導彈。</li>
        <li><b>2、 3、 4秒:</b> 在追上來的披薩側分攤波動炮。</li>
      </ul>
    </td>
    <td><img src="https://tuufless.github.io/FFXIV-Elemental-Raid-Macros/assets/images/ultimates/top/01/pantokrator_06.jpg"></td>
  </tr>
  <tr>
    <td>
      <p><b>10.</b> 第3組預兆（第1次分攤單點判定後）</p>
      <ul>
        <li><b>1號:</b> 重新回到小組。</li>
        <li><b>2號:</b> 脫離小組往場中移動準備引導預兆。</li>
      </ul>
    </td>
    <td><img src="https://tuufless.github.io/FFXIV-Elemental-Raid-Macros/assets/images/ultimates/top/01/pantokrator_07.jpg"></td>
  </tr>
  <tr>
    <td>
      <p><b>11.</b> 第2輪分攤與單點（第1輪分攤與判定後）</p>
      <ul>
        <li><b>2號:</b>往最遠的披薩移動。 </li>
      </ul>
    </td>
    <td><img src="https://tuufless.github.io/FFXIV-Elemental-Raid-Macros/assets/images/ultimates/top/01/pantokrator_08.jpg"></td>
  </tr>
  <tr>
    <td>
      <p><b>12.</b> 第2輪分攤與單點判定</p>
      <ul>
        <li><b>2號:</b> 預兆出現後移動並準備重新回到小組。</li>
      </ul>
    </td>
    <td><img src="https://tuufless.github.io/FFXIV-Elemental-Raid-Macros/assets/images/ultimates/top/01/pantokrator_09.jpg"></td>
  </tr>
</table>

此循環會再重複2次 (3號與4號需要各離開一次，小組會再承受2輪分攤)。


### Wave Cannons
Omega會瞄準 **最遠的** 2名玩家死刑，由坦克的無敵來吃下這個傷害。

Omega會瞄準 隨機 3名非坦玩家造成1次直線傷害，並在頭上會顯示紅色標記。

<table>
  <tr>
    <td width="50%">
      <p><b>16.</b> 雙坦在北集合，<b>離開</b> Omega的目標圈並打開無敵。</p>
      <p>這將南邊有更大的空間可以分散，其餘玩家 <b>站進</b> 目標圈。 
      </p>
      <p>3名非坦玩家將在第1輪單點波動炮中被選中。</p>
    </td>
    <td><img src="https://tuufless.github.io/FFXIV-Elemental-Raid-Macros/assets/images/ultimates/top/01/wave_cannons_01.jpg"></td>
  </tr>
  <tr>
    <td>
      <p><b>17.</b> 第1輪波動判定</p>
      <p>剩下3名玩家被標記為第2輪波動炮對象。</p>
    </td>
    <td><img src="https://tuufless.github.io/FFXIV-Elemental-Raid-Macros/assets/images/ultimates/top/01/wave_cannons_02.jpg"></td>
  </tr>
  <tr>
    <td>
      <p><b>17.</b> 第2輪波動炮判定</p>
      <p>判定後， Omega會讀條「原子射線」作為本階段狂暴。</p>
    </td>
    <td><img src="https://tuufless.github.io/FFXIV-Elemental-Raid-Macros/assets/images/ultimates/top/01/wave_cannons_03.jpg"></td>
  </tr>
</table>

---

## 常見問題

<details markdown=block>
<summary>
  <b>[全能之主]</b> 為什麼小組以北西南東分組而不是南北分組?
</summary>
<table>
  <tr>
    <td>
      <p>這是因為披薩的方向是基於Omega的面相。</p>
      <p>將小組直接放在南北的問題是，披薩是60度的範圍且每次旋轉30度，</p>
      <p>這意味著你有可能遇到如右圖一樣，發生模稜兩可無法判斷是否覆蓋南北的情況。</p>
      <p>在我們默認初始起跑點被覆蓋時永遠向 <b>順時針 </b> 旋轉，在上述情況明顯不是完美的判斷邏輯。</p>
      <p>透過將Omega面北後旋轉45度角作為初始點，在邏輯上永遠不會遇到難以判斷的狀況。</p>
    </td>
    <td><img src="https://tuufless.github.io/FFXIV-Elemental-Raid-Macros/assets/images/ultimates/top/01/pantokrator_faq.jpg"></td>
  </tr>
</table>
</details>
<details markdown=block>
<summary>
  <b>[全能之主]</b> 為什麼我們讓小組分攤在火追過來的方向而不是火前進的方向?
</summary>
<table>
  <tr>
    <td>
      <p>被火追分攤有以下幾個優點:</p>
      <ul>
        <li>只有1名玩家（單點導彈）需要注意披薩的旋轉方向。</li>
        <li>由於只有1名玩家在前面， 要閃躲的預兆數量只有1個，相對好閃躲。</li>
        <li>第1組導彈的預兆可以在Omega腳下引導，為隊伍提供更多空間。</li>
      </ul>
      <p>另外，追著火分攤有以下缺點：</p>
      <ul>
        <li>導彈的玩家有可能被 <em>3名</em> 玩家的預兆擋住回不去小組。</li>
        <li>發生問題時因為有3名玩家在前面放預兆除錯上也變得困難。</li>
      </ul>
    </td>
  </tr>
</table>
</details>

---

## 問題解決

<details markdown=block>
<summary>
  <b>[全能之主]</b> 為什麼有人總是把黃圈丟在小組的移動方向前?
</summary>
<table>
  <tr>
    <td>
      <p>檢查玩家是不是以同樣的方式移動。</p>
      <p>在全能之主中有 <b>2種</b> 去引導預兆。</p>
      <p>我們讓即將出去的單點玩家在分攤後再留下1個預兆後才離開小組(黃色路徑)。</p>
      <p>Haru Glory在他們固定隊則是更提前，在分攤後就讓需要遠離小組的人離開（綠色路徑）。</p>
      <p>如果上一個玩家是走黃色路徑下一個玩家走綠色路徑的話，就會發生走綠色路徑的玩家撞在黃色路徑玩家的預兆上，因為當綠色路徑玩家出去的時候黃色路徑玩家的預兆還沒有消失。</p>
      <p>Haru Glory的隊伍後來將路徑從黃色路徑調整成了綠色路徑。</p>
    </td>
    <td><img src="{{site.baseurl}}/assets/images/ultimates/top/01/pantokrator_movement.jpg"></td>
    <td><img src="{{site.baseurl}}/assets/images/ultimates/top/01/pantokrator_movement_fast.jpg"></td>
  </tr>
</table>
</details>
