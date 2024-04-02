🐳  → docker run --restart always \
  --name derper -p 12345:12345 -p 3478:3478/udp \
  -v /root/.acme.sh/xxxx/:/app/certs \
  -e DERP_CERT_MODE=manual \
  -e DERP_ADDR=:12345 \
  -e DERP_DOMAIN=xxxx \
  -e DERP_VERIFY_CLIENTS=true \
  -d ghcr.io/yangchuansheng/derper:latest
