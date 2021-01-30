# Darling repo

This is an unofficial repo containing .debs for darling.

It will be updated up to two times a week.

## Installing
```
# Update sources.list 
echo "deb https://github.com/JCWasmx86/unofficial_darling/raw/main debian main" | sudo tee -a /etc/apt/sources.list
# Add public key
wget https://raw.githubusercontent.com/JCWasmx86/JCWasmx86.github.io/master/jcwasmx86.pgp&&sudo apt-key add jcwasmx86.pgp&&rm jcwasmx86.pgp
# Install darling
sudo apt update&&sudo apt install darling
```

## Disclaimer

Use all of these files on your own risk.
The .deb files are just built by using:
```
git clone --recursive -b update-sources https://github.com/darlinghq/darling.git
cd darling
./tools/makedeb
```
After this, I'm applying the `compressBetter`(Has to be run as root) script to improve compression.

I did this to bring the filesize under 100MB, so github accepts it.
