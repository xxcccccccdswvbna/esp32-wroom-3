# esp32-wroom-3

ct1/
├── ct1.yaml                      # 1. 主入口
├── base/                         # 基础系统层
│   ├── wifi.yaml                 # 2. WiFi (安全)
│   ├── web.yaml                  # 3. Web Server
│   ├── sensors.yaml              # 4. 传感器
│   ├── text_sensors.yaml         # 5. 文本传感器
│   ├── outputs.yaml              # 6. GPIO 输出
│   ├── lights.yaml               # 7. LED 灯光
│   ├── physical_keys.yaml        # 8. 物理按键 (KEY1-4)
│   ├── globals_extra.yaml        # 9. 额外全局变量
│   ├── offline_script.yaml       # 10. 离线闪烁脚本
│   └── mqtt.yaml                 # 11. 巴法云 MQTT (安全)
├── core/                         # V2 核心架构层
│   ├── globals.yaml              # 12. V2 核心变量
│   ├── scripts.yaml              # 13. V2 核心脚本 (防抖/队列/发送)
│   ├── state.yaml                # 14. 状态中心 (State Center)
│   └── buttons.yaml              # 15. V2 控制按钮 (Toggle/重启)
├── data/                         # V2 数据层
│   └── packets.yaml              # 16. 纯抓包数据库
├── ble/                          # BLE 硬件层
│   ├── core.yaml                 # 17. BLE 基础配置
│   ├── tracker.yaml              # 18. BLE 扫描解析 (Dev3)
│   └── dev3.yaml                 # 19. Dev3 状态传感器
└── .github/
    └── workflows/
        └── build.yml             # 20. CI/CD 自动编译
