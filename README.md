
### **PWR Chain RPC Node Guide**

**Important Note**: This is the inaugural testnet launch. While we strive for perfection, there might be unforeseen issues. We appreciate all feedback, bug reports, or any other issues reported in our [Discord server](https://discord.gg/DJkcuy9SAg).

#### **Requirements**:
- **CPU**: Single Core
- **Memory**: 1 GB RAM
- **Disk**: 25 GB SSD
- **Open Ports**: 8085

#### **Setup on Ubuntu Server**:

1. **Update OS**: 
   ```bash
   sudo apt update
   ```

2. **Install Java**: 
   ```bash
   apt install openjdk-19-jre-headless
   ```

3. **Clone the PWR RPC  Node Repository**:
   ```bash
   git clone https://github.com/PWR-Labs/PWR-RPC-Node.git
   ```

4. **Navigate to the RPC Node Directory**:
   ```bash
   cd PWR-Validator-Node
   ```

5. **Run the RPC**:
   ```bash
   java -jar rpc.jar rpc <REQUEST_RATE_LIMIT> <REUEST_BAN_LIMIT>
   ```
Replace <REQUEST_RATE_LIMIT> and <REUEST_BAN_LIMIT> with your preffered values and you're all set.

6. **Running in the Background**:
   If you wish to run the node in the background, ensuring it remains active after closing the terminal, utilize the `nohup` command:
   ```bash
   nohup java -jar rpc.jar rpc <REQUEST_RATE_LIMIT> <REUEST_BAN_LIMIT> &
   ```

Congratulations, you've now set up and run your PWR RPC Node.
