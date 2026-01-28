# Conceptual-Logical-Data-Model---StreamVault

StreamVault is a startup company planning to launch a comprehensive digital media library platform that allows users to manage, organize, and stream their personal collections of movies, TV shows, music, documentaries, and podcasts. The company wants to differentiate itself by offering advanced features like collaborative playlists, detailed content metadata, social features, and sophisticated recommendation algorithms. StreamVault needs a database system to support the following core functionalities:

Users can create accounts with profiles containing personal information, preferences, and subscription details; users can also watch as guests without having an account or profile, but streaming is limited to 2 hours per month
The platform supports three subscription tiers: Basic ($1.99/month), Premium ($9.99/month), and Family ($14.99/month for up to 5 users) but prices may change
Users can follow other users and see their public playlists and reviews
The system must store detailed information about various media types: movies, TV shows (with seasons and episodes), music (albums and individual tracks), podcasts (series and episodes), and documentaries
Each content item has extensive metadata including title, release date, duration, genre(s), language(s), country of origin, and age rating
Users can create custom playlists that can contain mixed media types
Users can maintain a "watch later" list and track viewing progress
The system maintains viewing history with timestamps and device information
Users can rate content on a 5-star scale and write text reviews
Track streaming quality preferences per user (480p, 720p, 1080p, 4K)
Record device information for each streaming session (device type, IP address, bandwidth usage)
