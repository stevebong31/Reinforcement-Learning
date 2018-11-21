<pre><code>
import gym
env = gym.make("FrozenLake-v0") #환경 구성
observation = env.reset() #환경 초기화
for _ in range(1000):
    env.render() #디스플레이 출력
    action = env.action_space.sample() #액션 설정
    observation, reward, done, info = env.step(action) #액션이 수행했을 경우 돌아오는 데이터
    </code></pre>
