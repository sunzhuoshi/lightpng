env = Environment();
Export('env')
env.SConscript(dirs=['third_party/zlib', 'third_party/libpng'])
env.Program('lightpng', ['src/lightpng.cpp', 'src/PNGRead.cpp'],
        LIBS=['png', 'z'],
        LIBPATH=['third_party/zlib/', 'third_party/libpng/'],
        CPPPATH=['./src', 'third_party/zlib/', 'third_party/libpng/'],
        CCFLAGS=['-g']) 
