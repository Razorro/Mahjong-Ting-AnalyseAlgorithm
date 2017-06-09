# Mahjong-Ting-AnalyseAlgorithm
An algorithm that analyse whether a card list can be Hu or Ting

***
## 不带万能牌的听胡分析
通过深度优先遍历，将所有可能过滤掉，然后在枚举最后简单情况下的听胡分析  
常规胡牌时，牌的数量必定满足3N+2，N in {0,1,2,3,4}  

有两个情况，第一个是过滤掉所有吃碰可能，然后进行吃胡分析，此时，在不能进行吃碰的基础上，容易推出剩下的牌的数量在2,5时才有可能进行听或者胡牌  
另一个方向是，先把将牌挑出，然后过滤，再进行第一种情况下的分析，此时，在不能进行吃碰的基础上，容易推出剩下的牌的数量在0,3时才有可能进行听或者胡牌  

_userCard: 用户的手牌，用haspMap表示，key带牌牌的值，value代表这种牌的数量  
_tingCard: 能听的牌，也就是打出后进入听牌状态  
_huCard: 能胡的牌，听牌后可以胡的牌  
_isHu: 是否可胡  



## 带万能牌的听胡分析（后续再加）
