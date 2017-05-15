# SoundManager
#import "SoundManager.h" where you want to use sound.

// User below code for effect sound clip.
[[SoundManager sharedManager] prepareToPlay];
[[SoundManager sharedManager] playMusic:@"YOUR SOUND NAME" looping:NO];

// User below code for background sound.
[SoundManager sharedManager].allowsBackgroundMusic = YES;
[[SoundManager sharedManager] prepareToPlay];
[[SoundManager sharedManager] playMusic:@"YOUR SOUND NAME" looping:YES];

// Stop background sound
[[SoundManager sharedManager] stopMusic];
