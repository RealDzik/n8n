    curl -X POST \
      http://localhost:5678/webhook/youtube-downloader \
      -H "Content-Type: application/json" \
      -d '{
        "youtubeUrl": "https://www.youtube.com/watch?v=Ip_yWsGUF6c&t=10s"
      }'


curl -X POST http://localhost:5678/webhook-test/youtube-downloader -H "Content-Type: application/json" -d '{"youtubeUrl": "https://www.youtube.com/watch?v=Ip_yWsGUF6c&t=10s"}'

http://localhost:5678/webhook-test/youtube-downloader


curl -X POST http://localhost:5678/webhook-test/youtube-downloader -H "Content-Type: application/json" -d '{"youtubeUrl": "https://www.youtube.com/watch?v=Ip_yWsGUF6c&t=10s"}'

yt-dlp "{{$json.body.youtubeUrl}}"
yt-dlp --write-subs --sub-langs "zh-CN,en" -o "E:/download/%(title)s [%(id)s].%(ext)s" "{{$json.body.youtubeUrl}}"

yt-dlp --write-auto-subs --sub-langs "zh-CN,en" -o "E:/download/%(title)s [%(id)s].%(ext)s" "{{$json.body.youtubeUrl}}"

.venv\Scripts\Activate.ps1

pip install yt-dlp

pnpm start

$env:WEBHOOK_URL="http://localhost:5678/"; npx n8n start
$env:WEBHOOK_URL="http://localhost:5678/"; pnpm dev


npx n8n

    Get-Process | Where-Object { $_.ProcessName -like "*node*" -or $_.ProcessName -like "*pnpm*" -or $_.ProcessName -like "*turbo*" -or $_.ProcessName -like "*n8n*" } | Stop-Process -Force

rm -r -force node_modules
Remove-Item pnpm-lock.yaml
pnpm install
npm build


npx n8n
npm update -g n8n