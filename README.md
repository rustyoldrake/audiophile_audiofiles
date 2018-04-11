# audiophile_audiofiles
audiophile_audiofiles - audio files and scripts to edit them

Playing with my SOX
SoX is the Swiss Army knife of sound processing programs. A command line utility that can
convert various formats of computer audio files in to other formats. “It can also apply various
effects to these sound files, and, as an added bonus, SoX can play and record audio files on
most platforms”

http://sox.sourceforge.net/
Play source file
play jfk.wav

Speed Change - higher number speeds up - and pitch shifts too
sox jfk.wav jfk_speed.wav speed 1.33
sox jfk.wav jfk_speed3.wav speed 3 # speeds up quite a bit

Pitch Lift Up - Nasal
sox jfk.wav jfk_pitch.wav pitch 200

Pitch Drop - Throat
sox jfk.wav jfk_pitch.wav pitch -200

Speed Change without pitch shift
sox jfk.wav jfk_tempo.wav tempo -s 2.1

For OGG to WAV conversion needed to install via brew like below
brew install sox --with-lame --with-flac --with-libvorbis
then this worked - OGG to WAV
sox sample1.ogg sample1.wav

Pitch Shifting - the ‘down’ makes me sound like a super hero
sox sample1.wav sample1_pitchup.wav pitch 200
sox sample1.wav sample1_pitchdown.wav pitch -200

Sox Rocks!
