# AWS-Free-Tier-2025

### 🖥️ **EC2** 
**Mục tiêu:** Tạo và quản lý máy ảo trên AWS cloud

**📋 Các bước thực hiện:**

1. **Truy cập EC2 Console**
   ```
   AWS Console → Services → EC2 → Launch Instance
   ```

2. **Cấu hình Instance**
   - **Name:** `my-first-ec2`
   - **AMI:** Amazon Linux 2023 (Free tier eligible)
   - **Instance Type:** `t2.micro` (Free tier eligible)
   - **Key Pair:** Tạo mới hoặc sử dụng existing
   - **Security Group:** Default (SSH access)

3. **Launch và Connect**
   - Click **"Launch Instance"**
   - Đợi status **"Running"**
   - Test SSH connection (optional)

4. **Clean Up**
   - Terminate instance sau khi hoàn thành
   - Verify trong EC2 Console

**💰 Chi phí ước tính:** $0.0116/hour (sẽ được trừ từ credit)
**⏱️ Thời gian:** 15-20 phút
