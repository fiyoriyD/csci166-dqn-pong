# DQN on Pong (CSCI 166)

## Videos
### Early training (near-random)
<video src="videos/rl-video-episode-0.mp4" controls width="480"></video>

### Later training (~30k frames)
<video src="videos/rl-video-episode-1.mp4" controls width="480"></video>

> If the videos don’t render inline, use these direct links:  
> - Early: [videos/rl-video-episode-0.mp4](videos/rl-video-episode-0.mp4)  
> - Later: [videos/rl-video-episode-1.mp4](videos/rl-video-episode-1.mp4)

---

##  Project Notes
- **Environment:** `Pong-v4` (Gymnasium)
- **Algorithm:** DQN (replay buffer + target network, frame stacking)
- **Training so far:** ~30k frames for these clips

## Reflection
I chose **Pong** because it’s a classic Atari RL benchmark with simple rules and sparse/delayed rewards.  

**Early training:** behavior was almost random—frequent misses, strongly negative returns.  
**Later (~30k frames):** small but visible improvements: more consistent paddle movement and occasional successful returns. Performance is still weak, which is expected at this short horizon.

**Challenges:** sparse rewards and long credit assignment make learning slow.  
**Next steps:** I am **continuing training to ~300k frames** and will update this repo and my post with improved videos once training completes.
