# Check Image

- docker images

# Command

# example ที่เราจะ run (กรณีมีหลายไฟล์)

- docker build -t [node-server] -f ./Dockerfile .

# ถ้าเกิดเป็น Dockerfile อยู่แล้ว (ไม่ใช่ชื่ออื่น) สามารถย่อเหลือเพียงแค่

- docker build -t [node-server] .

# Run Container

- docker run [node-server]

# Run Container with map port

# เพิ่ม -d เพื่อให้สามารถ run background ได้

# map จาก port ภายนอกเข้าภายใน

- docker run -d -p 8000:8000 [node-server]

# Check printing of server with NAME

- docker logs [hardcore_volhard]

# Check Running Containner Process

- docker ps

# Quit Running Container Process with NAME

- docker rm -f [hardcore_volhard]

# Quit All Running Container Process

- docker rm -f $(docker ps -a -q)

---

# Build

# build container

- docker-compose up -d --build

# Close Compose

- docker-compose down

# Check Volumns

- docker volume ls

# Get into Container (VM) | MYSQL
- docker exec -it [db] bash
- mysql -u root -p
