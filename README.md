# mobile-eggbert-fna


## Init submodules

git submodule update --init --recursive
cd FNA &&  git submodule update --init --recursive
cd ../fnalibs &&  git submodule update --init --recursive && cd ..

## Apply patches

cd FNA && git apply ../FNA.patch
cd ../fnalibs && git apply ../fnalibs.patch && cd ..

## build

cd mobile-eggbert-fna && dotnet build

## Add libraries base on the platform

For Linux, add these files to directory mobile-eggbert-fna/mobile-eggbert-fna/bin/Debug/net4.0

## Copy directories Content and worlds to directory mobile-eggbert-fna/mobile-eggbert-fna/bin/

## Run the game

Go to mobile-eggbert-fna/mobile-eggbert-fna/bin/ and run:
On Linux: mono mobile-eggbert-fna.exe
On Windows: run directly mobile-eggbert-fna.exe
