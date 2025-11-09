# AI 本地化部署 docker+ollama+FastGPT+ONE API
## 1 docker

## 2 ollama

## 3 dmeta-embedding
### 3.1 测试API
```
curl "http://localhost:11434/api/chat" ^ 
--data "{""model"": ""qwen:0.5b"",""messages"":[{""role"": ""user"", ""content"": ""你是谁""}],""temperature"": 0.1, ""stream"": false}"
```

```
curl "http://localhost:11434/api/embeddings" ^
 -d "{""model"": ""shaw/dmeta-embedding-zh"",
  ""prompt"": ""天空是灰色的""
}"
```


```
curl "http://localhost:11434/api/embed"^ -d "{""model"": ""shaw/dmeta-embedding-zh"", ""input"": ""测试文本""}"
```
## 4 安装FastGPT及其依赖
docker配置文件下载

```
mkdir kbqa
cd kbqa 
curl -O https://harryai.cc/kbqa/docker-compose.yml
curl -O https://harryai.cc/kbqa/config.json
```

docker-compose up -d
