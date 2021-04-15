# Google-Cloud-AI-Your-Model-
Build and train your models  GSP324

#Explore Machine Learning Models with Explainable AI: Challenge Lab
#Build and train your models  GSP324

model = Sequential()
model.add(layers.Dense(200, input_shape=(input_size,), activation='relu'))
model.add(layers.Dense(50, activation='relu'))
model.add(layers.Dense(20, activation='relu'))
model.add(layers.Dense(1, activation='sigmoid'))
# The data will come from train_data and train_labels.
model.compile(loss='mean_squared_error', optimizer='adam', metrics=['accuracy'])
model.fit(train_data, train_labels, epochs=10, batch_size=2048, validation_split=0.1)

#2nd train your models  GSP324

limited_model = Sequential()
limited_model.add(layers.Dense(200, input_shape=(input_size,), activation='relu'))
limited_model.add(layers.Dense(50, activation='relu'))
limited_model.add(layers.Dense(20, activation='relu'))
limited_model.add(layers.Dense(1, activation='sigmoid'))
limited_model.compile(loss='mean_squared_error', optimizer='adam', metrics=['accuracy'])
# The data will come from limited_train_data and limited_train_labels.
limited_model.fit(limited_train_data, limited_train_labels, epochs=10, batch_size=2048, validation_split=0.1)
