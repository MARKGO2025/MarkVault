![[git常用命令.png]]
 # 提交前先拉取
git pull --rebase origin master  # 保持线性历史
git push

git pull --no-rebase origin master


 ls -al ~/my-ssh-keys
 id_ed25519
 id_ed25519.pub
cd storage/shared/000MARKYIN/'99 Mark Vault'
cd storage/shared/000MARKYIN/'99 xmind'
# 启动 ssh-agent

eval "$(ssh-agent -s)"
# 添加私钥
ssh-add ~/my-ssh-keys/id_ed25519
