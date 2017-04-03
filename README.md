# caffe_doc

1、install caffe on osx

#use homebrew to install the  necessary packages 
brew install -vd snappy leveldb gflags glog szip lmdb
brew tap homebrew/science
brew install hdf5 opencv
brew install protobuf boost wget

#download caffe source code
git clone https://github.com/bvlc/caffe.git
cd caffe
cp Makefile.config.example Makefile.config

#modify the config with CPU_ONLY
CPU_ONLY := 1

#complie
make -j

#errors
