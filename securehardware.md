# Hardware-intrinsic security primitives enabled by analogue state and nonlinear conductance variations in integrated memristors
integrated memristors，集成忆阻器；conductance variations，电导变化；Ionic Black Box，离子

He and his team are looking to put an extra layer of security on the growing number of internet- and Bluetooth-enabled devices with technology that aims to **prevent cloning**, the practice by which nodes in a network are replicated and then used to launch attacks from within the network.
A chip that deploys **ionic memristor technology**, it is an analog memory hardware solution to a digital problem.
Due to its nature, the chip is physically unclonable and can thus render the device invulnerable to hijacking(劫持), counterfeiting（伪造） or replication by cyber criminals.
 memristor, or memory resistor
 由忆阻器组成的电路会产生一种黑盒子，输出极难根据输入进行预测。
 circuits’ internal mechanisms are repeatable enough to be reliable.makes the relationship between inputs and outputs look random enough to the outside world

 Trojan，木马;fabrication process,制造过程，tampering attacks，篡改攻击

 The physical unclonable function (PUF) class, are a relatively new breed of hardware-based cryptographic primitives that rely on **inherent random variations in their fabrication process** to generate “secret keys” as a one-way function.
Practical PUF primitives based on CMOS and CMOS-integration-compatible technologies
nonvolatile memory crossbars based on resistive switching (ReRAM or memristive) devices基于电阻切换（ReRAM或忆阻）器件的非易失性存储器交叉开关
NIST statistical randomness test suite
 design workload,设计工作量，pre-silicon circuit protection，post-silicon phase
 emerging transistors, such as spin-transfer torque (STT) device, memristor, and spontronic domain wall
 # Security Based on Physical Unclonability and Disorder
 最近，人们越来越关注利用微观的，随机的和不可克隆的物理媒体无序来进行这种安全任务。在适用的情况下，利用无序可以带来有趣的优势：首先，它可以避免数字密钥永久存储在易受攻击的硬件中，有希望使得到的系统更能抵御侵入和恶意软件攻击。其次，随机物理紊乱具有非常难以克隆和伪造的自然特征：完全控制物理介质中的微米和纳米级制造变化是极其困难的，并且即使可能，也非常昂贵。第三，在物理系统中利用自然无序和熵有时可以使加密协议的安全性不依赖于通常的未经证实的数论理论假设，如因子分解和离散对数，为密码学创建了替代基础。
 nonvolatile memory (NVM)，非易失存储器；
 提取，估计或克隆以非易失性存储器中的数字存储的密钥的大量攻击
基于FPGA的可重配置设备，密钥的永久存储可能是一个问题

PUF是第二类重要的无序系统，可用于可靠的识别，认证，密钥存储和其他安全任务。简而言之，PUF是无序物理系统$S$，当由$C_i$表示的挑战（或输入，刺激）询问时，生成由$R_{C_i}$表示的唯一设备响应（或输出）。该响应应取决于所应用的挑战以及PUF的特定无序性和装置结构。 PUF定义中的不可克隆性要求是，**对于具有物理访问权限的对手来说，创建PUF的物理或软件克隆应该是难以处理的。**
Intel SGX

single instruction multiple data，单指令流多数据流
SSE（为Streaming SIMD Extensions的缩写）是由 Intel公司，在1999年推出Pentium III处理器时，同时推出的新指令集。如同其名称所表示的，SSE是一种SIMD指令集。
