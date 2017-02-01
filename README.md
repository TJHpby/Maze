# Maze
通过算法走出设定迷宫的程序
# 思路

设计两个类：       

`迷宫类`（MazeMap):                
>数据成员
* 墙壁字符  
* 通路字符  
* 迷宫数组
>成员函数
* 构造析构函数
* 数据封装函数      
* 迷宫绘制函数
* 迷宫边界检查函数 

`人`(Mazeperson):        
>数据成员
* 人型字符  
* 人的朝向  
* 当前位置 
* 下一位置 
* 行进速度
>成员函数
* 构造析构函数
* 数据封装函数      
* 不同方向行进函数
* 转弯函数 
* 开始函数

提示：动画控制函数

        void Mazeperson::gotoxy(int x,int y){                  
        COORD cd;                            
        cd.x=x;                                                 
        cd.y=y;                                                 
        HANDLE handle = GetStdHandle(STD_OUTPUT_HANDLE);                                                 
        SetConsoleCursorPosition(handle,cd);                                  
        };
