1. **启动服务：**

   ```bash
   docker-compose up -d
   ```

2. **修改`./velocity/velocity.toml`：**

   ```toml
   [servers]
   lobby = "lobby:25565"
   survival = "survival:25565"
   try = ["lobby"]

   player-info-forwarding-mode = "modern"
   forwarding-secret-file = "/secrets/forwarding.secret"
   ```

3. **重启 Velocity：**

   ```bash
   docker-compose restart velocity
   ```
