# -lgorithmic-structure-and-sound-composition


in_thread do
  sleep 20
  
  loop do
    4.times do
      use_synth :blade
      play :Fs3, release: 0.5
      sleep 0.25
      play :Gs3, release: 0.5
      sleep 0.25
      play :B3, release: 0.5
      sleep 0.25
      play :A3, release: 0.5
      sleep 0.25
    end
    4.times do
      use_synth :blade
      play :Fs3, release: 0.5
      play :Fs4, release: 0.5
      sleep 0.25
      play :Gs4, release: 0.5
      play :Gs3, release: 0.5
      sleep 0.25
      play :B4, release: 0.5
      play :B3, release: 0.5
      sleep 0.25
      play :A4, release: 0.5
      play :A3, release: 0.5
      sleep 0.25
    end
    4.times do
      use_synth :blade
      play :Fs3, release: 0.5
      play :Fs4, release: 0.5
      sleep 0.25
      play :Gs3, release: 0.5
      play :Gs4, release: 0.5
      sleep 0.25
      play :B3, release: 0.5
      play :B4, release: 0.5
      sleep 0.25
      play :A4, release: 0.5
      play :A4, release: 1
      sleep 0.25
    end
    sleep 16
  end
end

in_thread do
  
  sleep 4
  
  4.times do
    sample :drum_heavy_kick, amp: 0.8
    sleep 1
  end
  
  2.times do
    sample :drum_heavy_kick, amp: 0.8
    sleep 1
    sample :drum_snare_hard, amp: 0.8
    sleep 0.5
    sample :drum_heavy_kick, amp: 0.8
    sleep 0.2
    sample :drum_cymbal_pedal, amp: 0.8
    sample :drum_snare_soft, amp: 0.8
    sleep 0.3
  end
end

loop do
  use_synth :fm
  play :Fs3, release:0.3
  sleep 0.25
  play :Gs3, release:0.3
  sleep 0.25
  play :B3, release:0.3
  sleep 0.25
  play :A3, release:0.3
  sleep 0.25
end
