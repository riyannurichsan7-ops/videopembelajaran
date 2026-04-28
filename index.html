import React, { useState, useEffect, useRef } from 'react';
import { Play, Pause, SkipBack, SkipForward, MonitorPlay, Star, CheckCircle2, Clock, Check, Volume2, VolumeX } from 'lucide-react';

const scenes = [
  { id: 1, title: "Scene 1: Opening Kelas", time: "0:00 - 1:00" },
  { id: 2, title: "Scene 2: Apersepsi", time: "1:00 - 2:30" },
  { id: 3, title: "Scene 3: Perkenalan Media", time: "2:30 - 4:00" },
  { id: 4, title: "Scene 4: Demo Level 1", time: "4:00 - 6:00" },
  { id: 5, title: "Scene 5: Demo Level 2", time: "6:00 - 8:00" },
  { id: 6, title: "Scene 6: Demo Level 3", time: "8:00 - 10:00" },
  { id: 7, title: "Scene 7: Quiz Akhir", time: "10:00 - 12:00" },
  { id: 8, title: "Scene 8: Refleksi", time: "12:00 - 14:00" },
  { id: 9, title: "Scene 9: Penutup", time: "14:00 - 15:00" }
];

export default function App() {
  const [currentScene, setCurrentScene] = useState(0);
  const [isPlaying, setIsPlaying] = useState(false);
  const [gameScore, setGameScore] = useState(0);
  const [level1Answered, setLevel1Answered] = useState(false);
  const [isMuted, setIsMuted] = useState(true);
  const [toastMessage, setToastMessage] = useState("");
  const audioRef = useRef(null);

  // Auto-play logic
  useEffect(() => {
    let interval;
    if (isPlaying) {
      interval = setInterval(() => {
        setCurrentScene((prev) => {
          if (prev < scenes.length - 1) {
            setLevel1Answered(false); // Reset interactions
            return prev + 1;
          }
          setIsPlaying(false);
          return prev;
        });
      }, 5000); // Ganti adegan setiap 5 detik saat play
    }
    return () => clearInterval(interval);
  }, [isPlaying]);

  // Hilangkan pesan toast secara otomatis setelah 3 detik
  useEffect(() => {
    if (toastMessage) {
      const timer = setTimeout(() => setToastMessage(""), 3000);
      return () => clearTimeout(timer);
    }
  }, [toastMessage]);

  const handleNext = () => {
    if (currentScene < scenes.length - 1) {
      setCurrentScene(currentScene + 1);
      setLevel1Answered(false);
    }
  };

  const handlePrev = () => {
    if (currentScene > 0) {
      setCurrentScene(currentScene - 1);
      setLevel1Answered(false);
    }
  };

  const handleLevel1Answer = (isCorrect) => {
    if (isCorrect && !level1Answered) {
      setGameScore(gameScore + 20);
      setLevel1Answered(true);
    } else if (!isCorrect) {
      setToastMessage("Coba lagi! Itu bukan makhluk hidup. ❌");
    }
  };

  const toggleMute = () => {
    if (audioRef.current) {
      if (isMuted) {
        audioRef.current.volume = 0.25; 
        audioRef.current.play().then(() => {
          setIsMuted(false);
        }).catch(err => {
          console.log("Audio play error:", err);
          setToastMessage("Audio diblokir oleh browser di mode pratinjau ini. 🔇");
        });
      } else {
        audioRef.current.pause();
        setIsMuted(true);
      }
    }
  };

  // Render konten adegan berdasarkan currentScene
  const renderSceneContent = () => {
    switch (currentScene) {
      case 0:
        return (
          <div className="flex flex-col items-center justify-center h-full animate-fade-in text-center p-6 bg-yellow-50 rounded-2xl border-4 border-yellow-200">
            <h1 className="text-3xl font-bold text-blue-600 mb-4 bg-white px-6 py-2 rounded-full shadow-sm">
              📚 Pembelajaran IPAS: Pengenalan Makhluk Hidup
            </h1>
            <div className="flex items-end space-x-4 mt-8">
              <div className="text-8xl">👩‍🏫</div>
              <div className="bg-white p-4 rounded-2xl rounded-bl-none shadow-lg mb-8 max-w-md border-2 border-blue-100">
                <p className="text-xl font-semibold text-gray-700">
                  "Halo anak-anak! Hari ini kita akan belajar sambil bermain!" 👋
                </p>
              </div>
            </div>
            <div className="flex space-x-6 mt-4">
              <div className="text-5xl animate-bounce">👧</div>
              <div className="text-5xl animate-bounce delay-100">👦</div>
              <div className="text-5xl animate-bounce delay-200">👧</div>
            </div>
          </div>
        );
      case 1:
        return (
          <div className="flex flex-col items-center justify-center h-full p-6 bg-green-50 rounded-2xl border-4 border-green-200">
             <div className="bg-white p-4 rounded-2xl rounded-bl-none shadow-lg mb-6 border-2 border-green-100 self-start ml-12">
                <p className="text-xl font-semibold text-gray-700">
                  "Coba perhatikan gambar ini, mana yang termasuk makhluk hidup?" 🧐
                </p>
              </div>
              <div className="grid grid-cols-2 md:grid-cols-4 gap-6 w-full max-w-2xl mt-4">
                <div className="bg-white p-6 rounded-xl shadow-md flex flex-col items-center justify-center border-b-4 border-orange-400 transform transition hover:scale-105">
                  <span className="text-6xl mb-2">🐈</span>
                  <span className="font-bold text-gray-600">Kucing</span>
                </div>
                <div className="bg-white p-6 rounded-xl shadow-md flex flex-col items-center justify-center border-b-4 border-green-500 transform transition hover:scale-105">
                  <span className="text-6xl mb-2">🌳</span>
                  <span className="font-bold text-gray-600">Pohon</span>
                </div>
                <div className="bg-white p-6 rounded-xl shadow-md flex flex-col items-center justify-center border-b-4 border-gray-400 transform transition hover:scale-105">
                  <span className="text-6xl mb-2">🪨</span>
                  <span className="font-bold text-gray-600">Batu</span>
                </div>
                <div className="bg-white p-6 rounded-xl shadow-md flex flex-col items-center justify-center border-b-4 border-blue-400 transform transition hover:scale-105">
                  <span className="text-6xl mb-2">🧍‍♂️</span>
                  <span className="font-bold text-gray-600">Manusia</span>
                </div>
              </div>
          </div>
        );
      case 2:
        return (
          <div className="flex flex-col items-center justify-center h-full p-6 bg-purple-50 rounded-2xl border-4 border-purple-200">
            <h2 className="text-2xl font-bold text-purple-700 mb-6">Guru Memperkenalkan Game 💻</h2>
            <div className="bg-gray-800 p-4 rounded-t-xl w-full max-w-2xl border-b-4 border-gray-900 shadow-2xl relative">
               <div className="flex space-x-2 mb-3">
                 <div className="w-3 h-3 bg-red-500 rounded-full"></div>
                 <div className="w-3 h-3 bg-yellow-500 rounded-full"></div>
                 <div className="w-3 h-3 bg-green-500 rounded-full"></div>
               </div>
               <div className="bg-blue-400 rounded-lg h-64 flex flex-col items-center justify-center relative overflow-hidden">
                  <div className="absolute top-0 left-0 w-full h-full bg-[url('https://www.transparenttextures.com/patterns/cubes.png')] opacity-20"></div>
                  <h1 className="text-3xl font-extrabold text-white drop-shadow-md z-10 text-center px-4">
                    🌍 Petualangan Dunia <br/> Makhluk Hidup 🐾
                  </h1>
                  <button className="mt-6 bg-yellow-400 text-yellow-900 font-bold py-3 px-8 rounded-full shadow-lg border-b-4 border-yellow-600 hover:bg-yellow-300 transform transition hover:scale-105 z-10 flex items-center">
                    <Play className="mr-2" size={20} /> MULAI MAIN
                  </button>
               </div>
            </div>
            <div className="bg-gray-300 w-32 h-4 rounded-b-xl"></div>
          </div>
        );
      case 3:
        return (
          <div className="flex flex-col items-center justify-center h-full p-6 bg-green-100 rounded-2xl border-4 border-green-300 relative overflow-hidden">
            {/* Tema Hutan */}
            <div className="absolute top-2 right-4 flex items-center bg-white px-4 py-2 rounded-full shadow-sm font-bold text-blue-600">
              <Star className="text-yellow-400 mr-2 fill-current" /> Skor: {gameScore}
            </div>
            <h2 className="text-2xl font-bold text-green-800 mb-2 bg-white px-6 py-2 rounded-full shadow-sm">🌲 Level 1: Hutan Hijau</h2>
            <p className="text-xl font-semibold mb-6 text-gray-700">"Manakah yang termasuk makhluk hidup?"</p>
            
            <div className="flex space-x-6">
              <button onClick={() => handleLevel1Answer(true)} className={`p-6 rounded-xl shadow-md flex flex-col items-center justify-center border-b-4 border-orange-400 transform transition hover:scale-105 ${level1Answered ? 'bg-green-200' : 'bg-white hover:bg-orange-50'}`}>
                <span className="text-7xl mb-2">🐈</span>
                <span className="font-bold text-gray-700">Kucing</span>
              </button>
              <button onClick={() => handleLevel1Answer(false)} className="bg-white p-6 rounded-xl shadow-md flex flex-col items-center justify-center border-b-4 border-gray-400 transform transition hover:scale-105 hover:bg-gray-50">
                <span className="text-7xl mb-2">🪨</span>
                <span className="font-bold text-gray-700">Batu</span>
              </button>
              <button onClick={() => handleLevel1Answer(false)} className="bg-white p-6 rounded-xl shadow-md flex flex-col items-center justify-center border-b-4 border-amber-600 transform transition hover:scale-105 hover:bg-amber-50">
                <span className="text-7xl mb-2">🪑</span>
                <span className="font-bold text-gray-700">Kursi</span>
              </button>
            </div>

            {level1Answered && (
              <div className="absolute inset-0 bg-black bg-opacity-40 flex items-center justify-center z-20 animate-fade-in">
                <div className="bg-white p-8 rounded-3xl flex flex-col items-center shadow-2xl animate-bounce">
                  <Star className="text-yellow-400 w-24 h-24 fill-current mb-4" />
                  <h2 className="text-4xl font-extrabold text-green-500 mb-2">HEBAT!</h2>
                  <p className="text-xl font-bold text-gray-600">Kamu Benar!</p>
                </div>
              </div>
            )}
          </div>
        );
      case 4:
        return (
          <div className="flex flex-col items-center justify-center h-full p-6 bg-pink-50 rounded-2xl border-4 border-pink-200">
            <h2 className="text-2xl font-bold text-pink-700 mb-2 bg-white px-6 py-2 rounded-full shadow-sm">🌻 Level 2: Kebun Ceria</h2>
            <div className="bg-white p-8 rounded-2xl shadow-lg mt-6 w-full max-w-lg border-2 border-pink-100">
              <p className="text-xl font-bold text-gray-800 mb-6 text-center">Apa saja ciri-ciri makhluk hidup?</p>
              <div className="space-y-4">
                <div className="flex items-center p-3 bg-green-100 rounded-lg border border-green-300">
                  <CheckCircle2 className="text-green-600 mr-3" />
                  <span className="font-semibold text-green-800 text-lg">Bernapas 🌬️</span>
                </div>
                <div className="flex items-center p-3 bg-blue-100 rounded-lg border border-blue-300">
                  <CheckCircle2 className="text-blue-600 mr-3" />
                  <span className="font-semibold text-blue-800 text-lg">Tumbuh Besar 🌱</span>
                </div>
                <div className="flex items-center p-3 bg-purple-100 rounded-lg border border-purple-300">
                  <CheckCircle2 className="text-purple-600 mr-3" />
                  <span className="font-semibold text-purple-800 text-lg">Berkembang Biak 🐣</span>
                </div>
              </div>
              <div className="mt-6 flex justify-end">
                 <div className="bg-blue-50 text-blue-600 px-4 py-2 rounded-bl-none rounded-2xl text-sm font-semibold inline-block border border-blue-200">
                   "Ayo anak-anak, ikuti ibu guru ya!" 👩‍🏫
                 </div>
              </div>
            </div>
          </div>
        );
      case 5:
        return (
           <div className="flex flex-col items-center justify-center h-full p-6 bg-cyan-50 rounded-2xl border-4 border-cyan-200">
             <h2 className="text-2xl font-bold text-cyan-700 mb-2 bg-white px-6 py-2 rounded-full shadow-sm">🌊 Level 3: Sungai Pintar</h2>
             <p className="text-lg font-semibold mb-6 text-gray-600">Cocokkan kelompoknya!</p>
             
             <div className="flex w-full max-w-3xl justify-between items-center bg-white p-8 rounded-2xl shadow-md">
                {/* Kolom Kiri */}
                <div className="space-y-6">
                  <div className="bg-orange-100 p-4 rounded-xl border-2 border-orange-300 flex items-center font-bold text-xl"><span className="text-3xl mr-2">🐓</span> Ayam</div>
                  <div className="bg-green-100 p-4 rounded-xl border-2 border-green-300 flex items-center font-bold text-xl"><span className="text-3xl mr-2">🥭</span> Mangga</div>
                  <div className="bg-blue-100 p-4 rounded-xl border-2 border-blue-300 flex items-center font-bold text-xl"><span className="text-3xl mr-2">👧</span> Manusia</div>
                </div>

                {/* Garis Hubung (Simulasi Drag n Drop) */}
                <div className="flex flex-col space-y-12 text-gray-400">
                  <div className="w-16 h-1 bg-green-500 rounded-full"></div>
                  <div className="w-16 h-1 bg-green-500 rounded-full"></div>
                  <div className="w-16 h-1 bg-green-500 rounded-full"></div>
                </div>

                {/* Kolom Kanan */}
                <div className="space-y-6">
                  <div className="bg-gray-100 p-4 rounded-xl border-2 border-gray-300 border-dashed font-bold text-xl text-gray-600 w-40 text-center">Hewan</div>
                  <div className="bg-gray-100 p-4 rounded-xl border-2 border-gray-300 border-dashed font-bold text-xl text-gray-600 w-40 text-center">Tumbuhan</div>
                  <div className="bg-gray-100 p-4 rounded-xl border-2 border-gray-300 border-dashed font-bold text-xl text-gray-600 w-40 text-center">Manusia</div>
                </div>
             </div>
           </div>
        );
      case 6:
        return (
          <div className="flex flex-col items-center justify-center h-full p-6 bg-indigo-50 rounded-2xl border-4 border-indigo-200">
            <h2 className="text-2xl font-bold text-indigo-700 mb-6 bg-white px-6 py-2 rounded-full shadow-sm">⏱️ Quiz Akhir</h2>
            
            <div className="bg-gradient-to-br from-indigo-500 to-purple-600 p-10 rounded-3xl shadow-2xl text-center text-white transform transition-all animate-fade-in relative overflow-hidden">
               <div className="absolute top-0 right-0 p-4 opacity-20">
                 <Clock size={100} />
               </div>
               <h3 className="text-xl font-medium mb-2 opacity-90">Kuis Selesai!</h3>
               <div className="text-7xl font-black mb-4 tracking-tighter drop-shadow-lg">
                 95<span className="text-4xl text-indigo-200">/100</span>
               </div>
               <div className="bg-white text-indigo-600 px-6 py-3 rounded-full font-bold text-xl mb-4 shadow-md flex items-center justify-center">
                 <Check className="mr-2 font-bold" /> LUAR BIASA!
               </div>
               <p className="text-indigo-100">Semua siswa berhasil menjawab dengan baik!</p>
            </div>
          </div>
        );
      case 7:
        return (
          <div className="flex flex-col items-center justify-center h-full p-6 bg-yellow-50 rounded-2xl border-4 border-yellow-200">
             <h2 className="text-2xl font-bold text-yellow-800 mb-8 bg-white px-6 py-2 rounded-full shadow-sm">💡 Refleksi Pembelajaran</h2>
             
             <div className="grid grid-cols-1 md:grid-cols-2 gap-6 w-full max-w-4xl">
               <div className="bg-white p-6 rounded-2xl shadow-md border-l-8 border-blue-400">
                 <p className="font-bold text-gray-700 mb-2">👩‍🏫 Guru Bertanya:</p>
                 <ul className="list-disc pl-5 text-gray-600 space-y-2 font-medium">
                   <li>Apa saja ciri-ciri makhluk hidup?</li>
                   <li>Sebutkan contoh tumbuhan!</li>
                   <li>Mengapa batu bukan makhluk hidup?</li>
                 </ul>
               </div>
               
               <div className="bg-blue-50 p-6 rounded-2xl shadow-md border-l-8 border-green-400 flex flex-col justify-center">
                 <p className="font-bold text-gray-700 mb-2">👦👧 Siswa Menjawab:</p>
                 <div className="space-y-3">
                   <div className="bg-white p-3 rounded-lg text-sm font-semibold text-gray-700 shadow-sm">"Tumbuhan contohnya pohon mangga, Bu!"</div>
                   <div className="bg-white p-3 rounded-lg text-sm font-semibold text-gray-700 shadow-sm">"Batu tidak bisa bernapas dan tumbuh!"</div>
                 </div>
               </div>
             </div>
          </div>
        );
      case 8:
         return (
          <div className="flex flex-col items-center justify-center h-full p-6 bg-gradient-to-b from-blue-50 to-blue-200 rounded-2xl border-4 border-blue-300 text-center">
            <div className="text-6xl mb-6">👩‍🏫 👦 👧</div>
            <p className="text-2xl font-bold text-blue-800 mb-4 max-w-2xl leading-relaxed bg-white p-6 rounded-2xl shadow-lg border-2 border-blue-100">
              "Hari ini kita belajar bahwa makhluk hidup dapat bernapas, tumbuh, dan berkembang biak. Belajar akan lebih seru jika menggunakan media permainan."
            </p>
            <p className="text-xl font-medium text-gray-600 mb-8 animate-pulse">Sampai jumpa di pertemuan berikutnya! 👋</p>
            
            <div className="mt-4 pt-6 border-t-2 border-blue-300 w-full max-w-md">
              <h2 className="text-3xl font-extrabold text-blue-900 mb-2">Terima Kasih</h2>
              <p className="text-xl font-bold text-blue-700 bg-blue-100 py-2 px-6 rounded-full inline-block">Kelompok 7</p>
            </div>
          </div>
         );
      default:
        return null;
    }
  };

  return (
    <div className="min-h-screen bg-gray-100 p-4 md:p-8 flex items-center justify-center font-sans relative">
      {/* Toast Notification (Pengganti Alert yang diblokir) */}
      {toastMessage && (
        <div className="fixed top-10 left-1/2 transform -translate-x-1/2 bg-red-500 text-white px-6 py-3 rounded-full shadow-2xl z-[100] font-bold animate-bounce border-2 border-white">
          {toastMessage}
        </div>
      )}

      {/* Audio Element untuk Backsound Ceria */}
      <audio 
        ref={audioRef} 
        src="https://upload.wikimedia.org/wikipedia/commons/3/34/Kevin_MacLeod_-_Feelin_Good.ogg" 
        loop 
        preload="auto"
      />
      
      <div className="bg-white w-full max-w-5xl rounded-3xl shadow-2xl overflow-hidden border border-gray-200 flex flex-col h-[800px] relative">
        
        {/* Header - Video Title */}
        <div className="bg-gray-900 text-white p-4 flex items-center justify-between z-20 shadow-md">
          <div className="flex items-center space-x-3">
            <MonitorPlay className="text-blue-400" size={24} />
            <h1 className="font-bold text-lg hidden md:block">
              Simulasi Video: Game Edukasi "Petualangan Dunia Makhluk Hidup"
            </h1>
          </div>
          <div className="flex items-center space-x-4">
            {/* Tombol Toggle Backsound */}
            <button 
              onClick={toggleMute} 
              className="p-3 bg-gray-800 rounded-full hover:bg-gray-700 transition flex items-center text-gray-300 cursor-pointer relative z-50 border border-gray-700 shadow-sm"
              title={isMuted ? "Nyalakan Musik" : "Matikan Musik"}
            >
              {isMuted ? <VolumeX size={20} /> : <Volume2 size={20} className="text-green-400" />}
            </button>
            <div className="bg-gray-800 px-4 py-1 rounded-full text-sm font-semibold text-gray-300">
              Tugas UTS PGSD
            </div>
          </div>
        </div>

        {/* Video Screen Area */}
        <div className="flex-grow relative bg-gray-50 overflow-hidden">
          {renderSceneContent()}
        </div>

        {/* Video Controls & Timeline */}
        <div className="bg-white border-t border-gray-200 p-6 flex flex-col shadow-[0_-10px_20px_-10px_rgba(0,0,0,0.1)] z-10">
          
          {/* Scene Title Display */}
          <div className="text-center mb-4">
            <h3 className="font-bold text-xl text-gray-800">{scenes[currentScene].title}</h3>
            <p className="text-sm text-gray-500 font-medium">{scenes[currentScene].time}</p>
          </div>

          {/* Progress Bar */}
          <div className="w-full bg-gray-200 rounded-full h-3 mb-6 flex overflow-hidden">
             {scenes.map((scene, index) => (
                <div 
                  key={scene.id} 
                  className={`h-full transition-all duration-300 ${
                    index <= currentScene ? 'bg-blue-500' : 'bg-transparent'
                  }`}
                  style={{ width: `${100 / scenes.length}%`, borderRight: '1px solid rgba(255,255,255,0.3)' }}
                ></div>
             ))}
          </div>

          {/* Control Buttons */}
          <div className="flex items-center justify-center space-x-6">
            <button 
              onClick={handlePrev}
              disabled={currentScene === 0}
              className="p-3 text-gray-600 hover:text-blue-600 hover:bg-blue-50 rounded-full transition disabled:opacity-50 disabled:cursor-not-allowed"
            >
              <SkipBack size={28} />
            </button>
            
            <button 
              onClick={() => setIsPlaying(!isPlaying)}
              className="p-5 bg-blue-600 text-white rounded-full hover:bg-blue-700 hover:scale-105 transform transition shadow-lg flex items-center justify-center"
            >
              {isPlaying ? <Pause size={32} /> : <Play size={32} className="ml-1" />}
            </button>
            
            <button 
              onClick={handleNext}
              disabled={currentScene === scenes.length - 1}
              className="p-3 text-gray-600 hover:text-blue-600 hover:bg-blue-50 rounded-full transition disabled:opacity-50 disabled:cursor-not-allowed"
            >
              <SkipForward size={28} />
            </button>
          </div>
        </div>
        
      </div>
    </div>
  );
}
