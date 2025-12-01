![[git常用命令.png]]
 ls -al ~/my-ssh-keys
 id_ed25519
 id_ed25519.pub
cd storage/shared/000MARKYIN/'99 Mark Vault'
cd storage/shared/000MARKYIN/'99 xmind'
# 启动 ssh-agent

eval "$(ssh-agent -s)"
# 添加私钥
ssh-add ~/my-ssh-keys/id_ed25519
