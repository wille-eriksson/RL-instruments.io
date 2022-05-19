# Example of learning a Karplus-Strong melody

This is an example of how the parameters of the Karplus-Strong algorithm are learned over time to replicate an 8-note melody. The target audio consists of an E major arpeggio, with the first 4 notes being played normally and the last 4 notes being played in a staccato fashion. 

The prediction score, predicted parameters, produced STFT and audio are displayed for the untrained model and every 10.000 timesteps until a prediction score of 8.0 is reached.

------------------

## <ins>Target Audio</ins>

#### Karplus-Strong parameters

| Note      | Frequency | Pluck position | Loss factor | Amplitude |
| --------- | --------- | -------------- | ----------- | --------- |
| 1         | 82        |  0.5           |  0.996      | 0.5       |
| 2         | 123       |  0.5           |  0.996      | 0.5       |
| 3         | 165       |  0.5           |  0.996      | 0.5       |
| 4         | 208       |  0.5           |  0.996      | 0.5       |
| 5         | 208       |  0.1           |  0.91       | 1.0       |
| 6         | 165       |  0.1           |  0.91       | 1.0       |
| 7         | 123       |  0.1           |  0.91       | 1.0       |
| 8         | 82        |  0.1           |  0.91       | 1.0       |

#### STFT

<img src="figures/target.png" alt="drawing" width="600"/>

#### Audio

<audio controls>
  <source src="audio/target_audio.mp4" type="audio/wav">
</audio>

------------------

## <ins>Untrained prediction</ins>

#### Prediction score: 5.56

#### Karplus-Strong parameters

| Note      | Frequency | Pluck position | Loss factor | Amplitude |
| --------- | --------- | -------------- | ----------- | --------- |
| 1         | 82        |  0.1           |  0.91       | 0.5       |
| 2         | 195       |  0.3           |  0.91       | 1.0       |
| 3         | 240       |  0.1           |  0.91       | 1.0       |
| 4         | 282       |  0.1           |  0.91       | 1.0       |
| 5         | 195       |  0.3           |  0.996      | 1.0       |
| 6         | 195       |  0.3           |  0.91       | 1.0       |
| 7         | 237       |  0.3           |  0.91       | 0.5       |
| 8         | 149       |  0.3           |  0.91       | 1.0       |

#### STFT

<img src="figures/Predicted-melody-0-timesteps.png" alt="drawing" width="600"/>

#### Audio

<audio controls>
  <source src="audio/predicted_audio_0.mp4" type="audio/wav">
</audio>

------------------

## <ins>10.000 timesteps</ins>

#### Prediction score: 6.28

#### Karplus-Strong parameters

| Note | Frequency | Pluck position | Loss factor | Amplitude |
| ---- |-----------|----------------|-------------|-----------|
| 1    | 106       | 0.5            | 0.91        | 0.5       |
| 2    | 83        | 0.5            | 0.996       | 0.5       |
| 3    | 162       | 0.5            | 0.91        | 0.5       |
| 4    | 209       | 0.5            | 0.91        | 0.5       |
| 5    | 209       | 0.5            | 0.91        | 0.5       |
| 6    | 249       | 0.5            | 0.91        | 1.0       |
| 7    | 99        | 0.5            | 0.91        | 1.0       |
| 8    | 99        | 0.5            | 0.91        | 0.5       |

#### STFT

<img src="figures/Predicted-melody-10000-timesteps.png" alt="drawing" width="600"/>

#### Audio

<audio controls>
  <source src="audio/predicted_audio_10k.mp4" type="audio/wav">
</audio>

------------------

## <ins>20.000 timesteps</ins>

#### Prediction score: 6.65

#### Karplus-Strong parameters

| Note | Frequency | Pluck position | Loss factor | Amplitude |
| ---- |-----------|----------------|-------------|-----------|
| 1    | 241       | 0.5            | 0.91        | 0.5       |
| 2    | 130       | 0.5            | 0.996       | 0.5       |
| 3    | 164       | 0.5            | 0.91        | 0.5       |
| 4    | 209       | 0.5            | 0.91        | 0.5       |
| 5    | 209       | 0.5            | 0.91        | 1.0       |
| 6    | 164       | 0.5            | 0.91        | 1.0       |
| 7    | 99        | 0.1            | 0.91        | 1.0       |
| 8    | 99        | 0.5            | 0.91        | 1.0       |

#### STFT

<img src="figures/Predicted-melody-20000-timesteps.png" alt="drawing" width="600"/>

#### Audio

<audio controls>
  <source src="audio/predicted_audio_20k.mp4" type="audio/wav">
</audio>

------------------

## <ins>30.000 timesteps</ins>

#### Prediction score: 7.25

#### Karplus-Strong parameters

| Note | Frequency | Pluck position | Loss factor | Amplitude |
| ---- |-----------|----------------|-------------|-----------|
| 1    | 83        | 0.5            | 0.91        | 0.5       |
| 2    | 125       | 0.5            | 0.996       | 0.5       |
| 3    | 164       | 0.5            | 0.91        | 0.5       |
| 4    | 209       | 0.5            | 0.91        | 0.5       |
| 5    | 209       | 0.5            | 0.91        | 0.5       |
| 6    | 164       | 0.1            | 0.91        | 1.0       |
| 7    | 83        | 0.5            | 0.91        | 1.0       |
| 8    | 83        | 0.5            | 0.91        | 1.0       |

#### STFT

<img src="figures/Predicted-melody-30000-timesteps.png" alt="drawing" width="600"/>

#### Audio

<audio controls>
  <source src="audio/predicted_audio_30k.mp4" type="audio/wav">
</audio>

------------------

## <ins>40.000 timesteps</ins>

#### Prediction score: 7.78

#### Karplus-Strong parameters

| Note | Frequency | Pluck position | Loss factor | Amplitude |
|------|-----------|----------------|-------------|-----------|
| 1    | 83        | 0.5            | 0.996       | 0.5       |
| 2    | 125       | 0.5            | 0.996       | 0.5       |
| 3    | 164       | 0.5            | 0.996       | 0.5       |
| 4    | 209       | 0.5            | 0.91        | 0.5       |
| 5    | 209       | 0.1            | 0.91        | 0.5       |
| 6    | 164       | 0.1            | 0.91        | 1.0       |
| 7    | 121       | 0.1            | 0.91        | 1.0       |
| 8    | 83        | 0.1            | 0.91        | 1.0       |

#### STFT

<img src="figures/Predicted-melody-40000-timesteps.png" alt="drawing" width="600"/>

#### Audio

<audio controls>
  <source src="audio/predicted_audio_40k.mp4" type="audio/wav">
</audio>

------------------

## <ins>50.000 timesteps</ins>

#### Prediction score: 7.85

#### Karplus-Strong parameters

| Note | Frequency | Pluck position | Loss factor | Amplitude |
|------|-----------|----------------|-------------|-----------|
| 1    | 83        | 0.5            | 0.996       | 0.5       |
| 2    | 125       | 0.5            | 0.996       | 0.5       |
| 3    | 164       | 0.5            | 0.996       | 0.5       |
| 4    | 209       | 0.5            | 0.91        | 0.5       |
| 5    | 209       | 0.1            | 0.91        | 0.5       |
| 6    | 164       | 0.1            | 0.91        | 1.0       |
| 7    | 123       | 0.1            | 0.91        | 1.0       |
| 8    | 83        | 0.1            | 0.91        | 1.0       |

#### STFT

<img src="figures/Predicted-melody-50000-timesteps.png" alt="drawing" width="600"/>

#### Audio

<audio controls>
  <source src="audio/predicted_audio_50k.mp4" type="audio/wav">
</audio>

------------------

## <ins>60.000 timesteps</ins>

#### Prediction score: 7.92

#### Karplus-Strong parameters

| Note | Frequency | Pluck position | Loss factor | Amplitude |
|------|-----------|----------------|-------------|-----------|
| 1    | 83        | 0.5            | 0.996       | 0.5       |
| 2    | 125       | 0.5            | 0.996       | 0.5       |
| 3    | 164       | 0.5            | 0.996       | 0.5       |
| 4    | 209       | 0.5            | 0.996       | 0.5       |
| 5    | 209       | 0.1            | 0.91        | 1.0       |
| 6    | 164       | 0.1            | 0.91        | 1.0       |
| 7    | 123       | 0.1            | 0.91        | 1.0       |
| 8    | 82        | 0.1            | 0.91        | 1.0       |

#### STFT

<img src="figures/Predicted-melody-60000-timesteps.png" alt="drawing" width="600"/>

#### Audio

<audio controls>
  <source src="audio/predicted_audio_60k.mp4" type="audio/wav">
</audio>

------------------

## <ins>70.000 timesteps</ins>

#### Prediction score: 8.00

#### Karplus-Strong parameters

| Note | Frequency | Pluck position | Loss factor | Amplitude |
|------|-----------|----------------|-------------|-----------|
| 1    | 82        | 0.5            | 0.996       | 0.5       |
| 2    | 122       | 0.5            | 0.996       | 0.5       |
| 3    | 164       | 0.5            | 0.996       | 0.5       |
| 4    | 209       | 0.5            | 0.996       | 0.5       |
| 5    | 209       | 0.1            | 0.91        | 1.0       |
| 6    | 164       | 0.1            | 0.91        | 1.0       |
| 7    | 123       | 0.1            | 0.91        | 1.0       |
| 8    | 82        | 0.1            | 0.91        | 1.0       |

#### STFT

<img src="figures/Predicted-melody-70000-timesteps.png" alt="drawing" width="600"/>

#### Audio

<audio controls>
  <source src="audio/predicted_audio_70k.mp4" type="audio/wav">
</audio>






