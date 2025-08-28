# AWS-Free-Tier-2025

### 🖥️ **Task 1: Launch EC2 Instance** - $20 credit

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

### 🤖 **Task 2: Amazon Bedrock Playground** - $20 credit

**Mục tiêu:** Trải nghiệm AI/ML với foundation models

**📋 Các bước thực hiện:**

1. **Truy cập Bedrock Console**
   ```
   AWS Console → Services → Amazon Bedrock → Playgrounds
   ```

2. **Chọn Model**
   - **Recommended:** Claude 3 Haiku hoặc Titan Text
   - Click **"Select model"**

3. **Tạo Prompt**
   ```
   Prompt example:
   "Explain cloud computing in simple terms for beginners"
   ```

4. **Generate Response**
   - Click **"Run"**
   - Đọc và đánh giá response
   - Thử thêm 2-3 prompts khác

**💰 Chi phí ước tính:** $0.001-0.01 per request
**⏱️ Thời gian:** 10-15 phút

### 💰 **Task 3: Set up AWS Budgets** - $20 credit

**Mục tiêu:** Thiết lập monitoring và alerts cho chi phí

**📋 Các bước thực hiện:**

1. **Truy cập Budgets Console**
   ```
   AWS Console → Billing & Cost Management → Budgets
   ```

2. **Create Budget**
   - **Budget Type:** Cost budget
   - **Budget Name:** `Free-Tier-Monitor`
   - **Budget Amount:** $50 (25% của $200 credit)
   - **Time Period:** Monthly

3. **Set up Alerts**
   - **Alert 1:** 50% of budget ($25)
   - **Alert 2:** 80% of budget ($40)
   - **Alert 3:** 100% of budget ($50)
   - **Email:** Nhập email để nhận alerts

4. **Review và Create**
   - Kiểm tra tất cả settings
   - Click **"Create budget"**

**💰 Chi phí:** Miễn phí (2 budgets đầu tiên)
**⏱️ Thời gian:** 10-15 phút

### ⚡ **Task 4: Create Lambda Web App** - $20 credit

**Mục tiêu:** Xây dựng serverless web application

**📋 Các bước thực hiện:**

1. **Truy cập Lambda Console**
   ```
   AWS Console → Services → Lambda → Create function
   ```

2. **Create Function**
   - **Function Name:** `my-web-app`
   - **Runtime:** Python 3.12
   - **Architecture:** x86_64

3. **Add Function URL**
   - Trong function console → Configuration → Function URL
   - Click **"Create function URL"**
   - **Auth type:** NONE (for testing)
   - **CORS:** Enable

4. **Update Code**
   ```python
   import json
   
   def lambda_handler(event, context):
       return {
           'statusCode': 200,
           'headers': {
               'Content-Type': 'text/html',
           },
           'body': '''
           <html>
               <body>
                   <h1>Hello from AWS Lambda!</h1>
                   <p>My first serverless web app</p>
               </body>
           </html>
           '''
       }
   ```

5. **Test Function**
   - Click **"Deploy"**
   - Truy cập Function URL để test
   - Verify web page hiển thị

**💰 Chi phí ước tính:** $0.0000002 per request
**⏱️ Thời gian:** 20-25 phút

### 🗄️ **Task 5: Create RDS Database** - $20 credit

**Mục tiêu:** Thiết lập managed relational database

**📋 Các bước thực hiện:**

1. **Truy cập RDS Console**
   ```
   AWS Console → Services → RDS → Create database
   ```

2. **Database Configuration**
   - **Engine:** MySQL
   - **Version:** 8.0 (latest)
   - **Template:** Free tier
   - **DB Instance:** `db.t3.micro`

3. **Settings**
   - **DB Name:** `myfreetierdb`
   - **Master Username:** `admin`
   - **Password:** Tạo strong password
   - **VPC:** Default
   - **Public Access:** No

4. **Additional Configuration**
   - **Initial Database Name:** `testdb`
   - **Backup:** 7 days retention
   - **Monitoring:** Enable Enhanced Monitoring

5. **Create và Verify**
   - Click **"Create database"**
   - Đợi status **"Available"** (5-10 phút)
   - Test connection (optional)

6. **Clean Up**
   - Delete database sau khi hoàn thành task
   - Disable backup để tránh charges

**💰 Chi phí ước tính:** $0.017/hour
**⏱️ Thời gian:** 30-40 phút (bao gồm waiting time)

### 🎉 **Xác nhận hoàn thành**

**Cách kiểm tra credit:**
1. Truy cập [AWS Billing Console](https://console.aws.amazon.com/costmanagement/)
2. Vào **"Credits"** section
3. Verify tổng credit = $200

**Timeline hoàn thành:**
- **Task 1-3:** Có thể hoàn thành trong 1 ngày
- **Task 4-5:** Cần thêm 1 ngày để careful testing
- **Tổng thời gian:** 2-3 ngày

---
