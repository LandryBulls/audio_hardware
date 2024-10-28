# 🎙️ Audio Hardware for Naturalistic Conversation Research 

> *"Because your research questions probably don't include 'what's that weird buzzing sound?'"*

**Landry Bulls** ([@LandryBulls](https://github.com/LandryBulls))  
[SCRAP Lab](http://scraplab.org/)  

**Created:** October 2024

This guide contains information about the audio hardware used in [SCRAP Lab](http://scraplab.org/) for multi-person conversation research. Our setup is designed to record high-quality audio from multiple participants wearing face-mounted microphones during natural conversations. Whether you're studying linguistics, psychology, or just want to capture crystal-clear multi-person audio, this guide has got you covered! 🎯

## 🛠️ Hardware Setup

Our setup is designed to capture isolated, single-speaker audio from each participant in close-quarters conversation, saving everything as perfectly synchronized .WAV files to an SD card. The entire setup can be assembled into a portable rack that can be carried or rolled around (think of it as your mobile conversation-recording command center! 🚀).

While we use the wireless version described below, a more budget-friendly "hard-wired" setup is possible if participants will remain stationary. Here's what you'll need:

### Essential Components

#### 1. Face-Worn Cardioid Microphones (One per participant) 🎭
- **Option A:** [Countryman E6](https://www.sweetwater.com/store/detail/E6DW5L2SR--countryman-e6-directional-earset-for-sennheiser-speaking-beige-2mm) (Untested but promising)
- **Option B:** [DPA 4088](https://www.bhphotovideo.com/c/search?Ntt=Dpa%204088) (Our tried-and-true choice)

#### 2. Multi-Channel Wireless System 📡
You'll need a receiver system with:
- Multi-channel receiver unit
- Bodypack transmitters (one per participant)
- Recommended: [Nady 4w-1ku](https://www.bhphotovideo.com/c/product/1150753-REG/nady_4w_1ku_hm_10_black_4w_1ku_quad_uhf_wireless.html) 
  > Perfect for conversation research without the overkill of professional theater equipment!

#### 3. Digital Audio Recorder/Interface 💾
Choose based on your participant count:
- **For larger groups:** [Zoom LiveTrak L-8](https://www.bhphotovideo.com/c/product/1503664-REG/zoom_l_8_livetrak_l_8_8_channel_digital.html) (Supports 8 participants)
- **For pairs/mobile:** [Zoom H6](https://www.bhphotovideo.com/c/product/1805576-REG/zoom_h6essential_32_bit_float.html)

#### 4. Supporting Equipment 🔌
- **TRS Cables:** [Hosa TRS cables](https://www.bhphotovideo.com/c/product/828467-REG/Hosa_Technology_HSS_001_5_HSS_001_5_Balanced_1_4_TRS.html) (One per channel)
  > Pro tip: Get well-shielded, short (1-2 ft) cables to minimize interference!
- **Storage:** [SanDisk 128GB SD card](https://www.bhphotovideo.com/c/product/1692696-REG/sandisk_sdsdxxd_128g_ancin_128gb_extreme_pro_uhs_i.html) (Have extras!)
- **Adapters:** [Various mic-to-receiver adapters](https://www.bhphotovideo.com/c/product/828468-REG/Hosa_Technology_GMP_467_3_5mm_TRS_to_1_4.html)
- **Power:** [SurgeX Power Conditioner](https://www.sweetwater.com/store/detail/SXDS208--surgex-sx-ds-208-defender-series-8-outlet-power-conditioner)
- **Optional but recommended:** [Gator Cases Rack](https://www.bhphotovideo.com/c/product/1027581-REG/gator_cases_gr_4s_4_space_shallow_rack.html)

## 📊 Signal Flow

```mermaid
graph LR
    A[Microphones] -->|Audio| B[Transmitters]
    B -->|Wireless| C[Receiver]
    C -->|TRS| D[Recorder]
    D -->|Digital| E[SD Card]
```

### Channel Configuration
- Each transmitter must be set to match its corresponding channel on the receiver
- Based on our testing, FM channels should be spaced at least 4 channels apart to prevent cross-talk and interference
  > For example, with 4 participants, you might use channels 1, 5, 9, and 13 to ensure clean separation

## 🔧 Additional Tools
Need to clean up your recordings or sync with video? Check out:
- [This script](https://github.com/LandryBulls/voicolate/blob/main/voicolate/isolate.py) for isolating individual microphone channels for enhanced separation
- [This script](https://github.com/LandryBulls/voicolate/blob/main/voicolate/transcribe.py) for using WhisperX to transcribe your audio files
- Functions in [This script](https://github.com/LandryBulls/multidata/blob/main/alignment/align.py) for aligning audio with video files (you will need to adjust the code to fit your specific setup). 

## 📝 Quick Tips
- Always test your wireless setup before recording
- Keep spare SD cards handy
- Monitor battery levels in transmitters
- Consider ambient noise in your recording space
- Use good cable management to prevent interference 

---
*Happy Recording! 🎉*

> For questions or contributions, feel free to open an issue or pull request!

## 📝 Citation

If you use this setup in your research, please cite as:

```bibtex
@misc{YourLastName2024audio,
  author = {Your Full Name},
  title = {Audio Hardware for Naturalistic Conversation Research},
  year = {2024},
  publisher = {GitHub},
  url = {https://github.com/LandryBulls/RepoName}
}
```