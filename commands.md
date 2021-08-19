# Lightweight GAN

## Train
`lightweight_gan --data data/marquez --name marquiz_1 --batch-size 16 --gradient-accumulate-every 4 --num-train-steps 200000 --amp True`

## Monitor GPU
`watch -n 1 nvidia-smi`

## Split video into images
`ffmpeg -i input.mp4 %d.png`
One image every second
`ffmpeg -i input.mp4 -vf fps=1 out%d.png`


## Generate interpolation
`lightweight_gan --name dignidad_1 --generate-interpolation`


