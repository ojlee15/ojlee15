- 👋 Hi, I’m @ojlee15
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
ojlee15/ojlee15 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

#! /bin/bash

os_info=$(cat /etc/os-release)

echo "\"server\":{"

name=$(echo "$os_info" | grep "NAME" | head -n 1 | cut -d '=' -f 2)
echo \        \"name\":"$name"

version=$(echo "$os_info" | grep "VERSION" | head -n 1 | cut -d '=' -f 2)
echo \        \"version\":\""$version"\"

echo },
