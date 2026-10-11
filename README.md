# ♟ Unbeatable Chess

لعبة شطرنج في الطرفية ضد بوت قوي جدًا مبني على محرك Stockfish.

## التثبيت
```bash
pip install -r requirements.txt
# ثم ثبّت Stockfish:
#   Windows: حمّله من https://stockfishchess.org/download/
#   macOS:   brew install stockfish
#   Linux:   sudo apt install stockfish
```

## التشغيل
الواجهة الرسومية (اضغط على القطعة ثم على المربع الهدف، R لإعادة اللعب):
```bash
python gui.py
python gui.py --color black
```
الواجهة النصية:
```bash
python main.py                      # تلعب بالأبيض
python main.py --color black        # تلعب بالأسود
python main.py --time 2             # بوت أقوى (تفكير أطول)
python main.py --engine /path/to/stockfish
```
يمكنك أيضًا ضبط متغير البيئة `STOCKFISH_PATH`.

أدخل الحركات بصيغة SAN (`Nf3`) أو UCI (`g1f3`).

## الترخيص
Stockfish مرخّص بـ GPLv3، وهذا المشروع لا يضمّن ملفاته، فقط يستدعيه.
