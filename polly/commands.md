aws polly describe-voices --language-code en-GB

aws polly synthesize-speech --output-format mp3 --text 'Hello, World' --voice-id Justin test.mp3

aws polly put-lexicon --name w3c --content file://example.pls

aws polly synthesize-speech --lexicon-names w3c --output-format mp3 --text 'Hello, my name is W3C' --voice-id Justin test-w3c.mp3

aws polly start-speech-synthesis-task --output-format mp3 --output-s3-bucket-name  s3-polly-test --text "Hello World" --voice-id Justin
