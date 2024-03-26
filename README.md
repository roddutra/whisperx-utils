# How to use WhisperX on Mac (Silicon)

```bash
whisperx source_files/output_audio_file.mp3 --compute_type int8 --language en --output_dir outputs --print_progress True
```

> Note: if you know the language of the audio, save some time by providing it using `--language en` for example.

## Speaker Diarization

> Note: if you know the number of speakers in the audio, use the `--min_spearkers` and `--max_speakers` params.
> You also need to provide your HugginFace token after `--hf_token` (get it [here](https://huggingface.co/settings/tokens))

```bash
whisperx source_files/output_audio_file.mp3 --compute_type int8 --diarize --min_speakers 2 --max_speakers 3 --language en --hf_token YOUR_HF_TOKEN_HERE --output_dir outputs --print_progress True
```

## Issues

Refer to the WhisperX [repository page](https://github.com/m-bain/whisperX) for more details.
