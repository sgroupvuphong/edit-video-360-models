# Edit Video 360 — mô hình lời thoại

Bản PhoWhisper (VinAI) chuyển sang định dạng ggml của [whisper.cpp](https://github.com/ggml-org/whisper.cpp), lượng tử hóa q8_0, dùng cho Edit Video 360.

- Mô hình gốc: [vinai/PhoWhisper](https://huggingface.co/vinai) — giấy phép BSD-3-Clause, xem `LICENSE-PhoWhisper`.
- Chuyển đổi: `whisper.cpp/models/convert-h5-to-ggml.py`, rồi `whisper-quantize ... q8_0`.
- Tệp nằm ở mục Releases. Ứng dụng kiểm SHA-256 từng tệp trước khi dùng.

| Tệp | Kích thước (byte) | SHA-256 |
| --- | --- | --- |
| PhoWhisper-tiny-q8_0.bin | 43537450 | `80fc2fe4da49a0244c86c1f7c5ce34f48568b19829199808ad7a696bec5606ff` |
| PhoWhisper-base-q8_0.bin | 81768602 | `9e78100d845978524462f17c2a2f22770e288393719973056033526335621d2a` |
| PhoWhisper-small-q8_0.bin | 264464624 | `df4d0ea0551a82282a3e32748388a26423c3cfa635aaec47741d55f6e99c1254` |
| PhoWhisper-medium-q8_0.bin | 823369796 | `22e687c11ebc3753e3110ee8a21a1dda9bbf93f9c0c6e931724b2603ba4f4970` |
| PhoWhisper-large-q8_0.bin | 1656129708 | `d72b0693d332453c79af9e56a94bd4768fa2e7dc055afacc86fe002a5a9841ad` |
