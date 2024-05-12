# Tank
这是一个临时拷贝的公开仓库，保存了一个使用Java制作的坦克大战网络游戏。  
本项目包含客户端和服务器端的功能实现，构建了完整的通信逻辑、多线程的游戏控制逻辑和图像绘制逻辑。  
  
- **并发**：  
  - 客户端的model和socket分别占据一个线程，使用线程池进行管理。   
  - 服务器端的model和selector分别占据一个线程，enemycreater占据一个线程，每一个具有run方法的Actor也都占据一个线程使用线程池进行管理。   
  - 【j05并发】 https://www.bilibili.com/video/BV1Rb4y137i6/?share_source=copy_web&vd_source=b96fbb898de9158b72bfd51f44c61e2a  
- **构建**：  
  - 使用Maven进行了自动构建  
- **测试**：  
  - 使用Maven进行了自动测试  
- **IO**：  
  - 实现了各种游戏保存功能，除地图加载由于地图实现的逻辑无法有效被加入整个逻辑，其余功能都得到了良好的实现。  
  - 【j05IO：地图保存与进度保存/进度加载】 https://www.bilibili.com/video/BV1tb4y137uL/?share_source=copy_web&vd_source=b96fbb898de9158b72bfd51f44c61e2a  
  - 【j05IO：游戏录制与回放功能展示】 https://www.bilibili.com/video/BV1DC4y1M7k9/?share_source=copy_web&vd_source=b96fbb898de9158b72bfd51f44c61e2a  
- **网络通信**：
  - 使用NIO的形式实现了网络通信，可支持n个客户一同游戏（为美观起见n设置为了小于6，不然界面就放不下了）
  - 【J05网络通信：多个客户端展示】 https://www.bilibili.com/video/BV1CQ4y1u7ED/?share_source=copy_web&vd_source=b96fbb898de9158b72bfd51f44c61e2a
