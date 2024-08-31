1. Download and install Node.js v. 10.15.3 from here: https://nodejs.org/download/release/v10.15.3/node-v10.15.3-x64.msi

2. Unzip "Tag Cloning Tools.7z". Copy and paste the LD Tag Cloning folder that you'll find inside to your Program Files folder to make it work instantly. Otherwise, you'll have to make changes to the files to make it work properly. You can create batch files that are suitable for your own folders based on the instructions in the Material folder. Everything you need is included in that folder, so that you won't have to download anything, but the sources are the following:
node-ld-master: https://github.com/bettse/node-ld
Node.js v10.15.3: https://nodejs.org/download/release/v10.15.3/node-v10.15.3-x64.msi
Advanced BAT to EXE Converter: https://www.battoexeconverter.com/

3. Once you open each program (depending on whether you want to write characters or vehicles, use LEGO Dimensions Character Tag Cloning.exe or LEGO Dimensions Vehicle Tag Cloning.exe respectively), you'll get a prompt asking you to type the NFC tag's UID. To get this, you need to have MIFARE++ Ultralight installed in your android phone (if anyone knows about an iOS alternative, let me know). You might not find this app in google play, so use a trusted website to download it as an apk and manually install it. Turn on the NFC in your phone and once installed, open MIFARE++ and use it to read one of your NFC tags. The UID is the first 6 digits from page 0 and all the 8 digits from page 1. For example, Page 0: 1D72E007, Page 1: 68031080, then the UID is 1D27E068031080. There's also an app called MIFARE Classic Tool, which you can probably find in Google Play Store and once you scan a tag with your phone, it immediately gives you the UID, so it saves time. So, scan a tag, get its UID and type it in the prompt.
   
4. When you click enter, you'll get a list of all available characters (or vehicles, depending on the bat file you chose before). Next to each character, there's be a series of digits, which you need to write to your NFC tag. Using MIFARE++ Ultralight, you can easily do so by reading a tag and then editing the specific pages that you need to change. Each tag has its own UID. You can't just input a random UID and write all tags based on that, because it won't work. You'll have to type each tag's specific UID every time you need to write a new character/vehicle. To write the tags, simply press write. Make sure to check my tips on the writing process below.

The pages that LEGO Dimensions always reads are 35, 36, 37, 38 and 43, so don't mind about the rest, the game won't read them. The PC program won't give you info on page 35 and 38, so make sure to read what I'm saying here:
Make sure that Page 35 is ALWAYS just 8 zeroes with no other digits in-between, no matter if you're writing characters or vehicles.
If you're writing characters, the pages you'll always have to change are 36, 37 and 43. You must change these pages to match the information given by the PC program.
If you're writing vehicles, the only pages you'll have to change are 38 and 43. In Page 38 in vehicles, you must always delete the 4th zero and replace it with a 1. That's how the game knows that this is supposed to be a vehicle and not a character. In page 43, just type what the PC program says for that page. You don't even have to search for the specific vehicle you want, as page 43 will always be the same for a specific UID, but NOT for all UIDs. This will register as a LEGO Dimensions vehicle, but to actually use it in the game you'll need a second tag in which you must write the character that the vehicle is associated to. For example, to use the Invisible Jet, you'll first need to have a tag with Wonder Woman written on it. When you boot the game, place the tag with the character in your toypad, but DO NOT place the vehicle there yet. Wait until the game gives you instructions to build the character's vehicle. If it doesn't, hold the triagle button and select "Building Instructions" from the menu. Just skip the instructions and once the game asks to write this vehicle to its toypad, select yes and then place the vehicle tag where it asks you to. If you've written everything correctly, the game will rewrite the tag and the vehicle will appear. Long story short, you can't write specific vehicles, only tags that register as blank vehicles in the game that can only be used in combination with their associated character.

Now, you can write anything you want and use it in LEGO Dimensions.

(Ignore this mess of a "source code")
