学习笔记

一、泛型递归与树的递归

递归 Recursion

递归 - 循环，通过函数体来进行的循环
类似于盗梦空间，向下进入到不同梦境中，向上又回到原来一层，每一层的环境和周围的人都是一份拷贝，主角等几个人穿越不同层级的梦境（发生和携带变化）

牢记模板！！！
Java 代码模版
public void recur(int level, int param) {
  // terminator  
  if (level > MAX_LEVEL) {
    // process result      
    return; 
  }
  // process current logic  
  process(level, param);  
  
  // drill down  
  recur( level: level + 1, newParam);  
  
  // restore current status  
}

思维要点：
1.	不要人肉进行递归（最大误区） 
2.	找到最近最简方法，将其拆解成可重复解决的问题（重复子问题） 
3.	数学归纳法思维

二、分治与回溯

分治 Divide & Conquer

回溯 Backtracking

回溯法采用试错的思想，它尝试分步的去解决一个问题。在分步解决问题的过程中，当它通过尝试发现现有的分步答案不能得到有效的正确的解答的时候，它将取消上一步甚至是上几步的计算，再通过其它的可能的分步解答再次尝试寻找问题的答案。 

回溯法通常用最简单的递归方法来实现，在反复重复上述的步骤后可能出现两种情况：
•	找到一个可能存在的正确的答案； 
•	在尝试了所有可能的分步方法后宣告该问题没有答案。

在最坏的情况下，回溯法会导致一次复杂度为指数时间的计算。

还得继续肝！太南了！Orz...

