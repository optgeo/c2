task :download do
  sh <<-EOS
curl -o docs/index.html https://optgeo.github.io/14321/index.html
curl -o docs/style.json https://optgeo.github.io/14321/style.json
curl -o docs/optimal_bvmap-v1.pmtiles https://cyberjapandata.gsi.go.jp/xyz/optimal_bvmap-v1/optimal_bvmap-v1.pmtiles
  EOS
# replace 14321.pmbtiles with optimal_bvmap-v1.pmtiles in style.json
end

task :add do
  sh <<-EOS
ipfs add --recursive docs
  EOS
end
