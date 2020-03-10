# Rearrangement-algorithm

This is an algorithm that determines where an object should be rearranged. 

## Problem Description

+ Environment : 목표물을 잡기 위해 장애물들을 치워야 하는 복잡한 환경.
+ Goal : 효율적인 공간의 활용을 통한 최소한의 장애물 재배치로 목표물에 도달.
+ Method : 장애물을 놓을 수 있는 빈 공간들을 통한 후보공간 생성, 이중 가장 효율적인 공간활용이 가능한 후보 결정

## Module

INPUT, OUTPUT에 쓰이는 사물정보란 물체의 이름, 위치, 크기가 포함된 msg 형태입니다.

### **INPUT**
+ 환경정보 : workspace 내에 있는 책상, 등 치워지지 않는 물체의 사물정보 (name, pose(position and orientation), scale(x,y,z))
+ 장애물 : workspace 내에 있는 움직일 수 있는 물체들 중 목표물을 제외한 나머지 물체들에 대한 사물정보
+ 목표물 : 목표물에 대한 사물 정보

### **OUTPUT**
+ 재배치 위치 : 재배치가 필요한 물체의 사물정보 및 재배치 위치

### **Preliminaries**
+ Accessibility check : To check if an object (or a candidate slot) in clutter is accessible by the robot end-effector *[ref-paper](https://ieeexplore.ieee.org/abstract/document/8793616)*
+ Relocate order finder : To determine the sequence of objects to be relocated *[ref-paper](https://arxiv.org/abs/1907.03956)*



## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)
