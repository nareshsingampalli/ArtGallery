# ArtGallery

In this project, we will build a Spring Boot application to serve as the backend for the 'Art Gallery' platform. 'Art Gallery' is a digital space where art enthusiasts can delve deep into the world of art pieces, their creators, and the galleries that showcase them.

Within 'Art Gallery', there are three key entities: Art, Artist, and Gallery. The Art entity establishes a Many-to-One relationship with the Artist, signifying that an artist can create multiple art pieces, but each art piece is associated with a single artist. Additionally, the Artist entity forms a Many-to-Many relationship with the Gallery entity, indicating that an artist can exhibit their artworks in multiple galleries, and similarly, a gallery can showcase works from multiple artists.

Implementation Files
Create a database that contains four tables art, artist, gallery, and artist_gallery using the given database schema.

You can refer to this session, for creating a database.

Create the SQL files and compose accurate queries to run the application. Inaccurate SQL files will result in test case failures.

Database Schema
Note
Use only art, artist, gallery, and artist_gallery as the table names in your code.

Completion Instructions
Artist.java: The Artist class should contain the following attributes.

Attribute	Type
artistId	int
artistName	String
genre	String
galleries	List<Gallery>
ArtistRepository.java: Create an interface containing the required methods.
ArtistJpaService.java: Update the service class with logic for managing artist data.
ArtistController.java: Create the controller class to handle HTTP requests.
ArtistJpaRepository.java: Create an interface that implements the JpaRepository interface.

Art.java: The Art class should contain the following attributes.

Attribute	Type
artId	int
artTitle	String
theme	String
artist	Artist
ArtRepository.java: Create an interface containing the required methods.
ArtJpaService.java: Update the service class with logic for managing art data.
ArtController.java: Create the controller class to handle HTTP requests.
ArtJpaRepository.java: Create an interface that implements the JpaRepository interface.

Gallery.java: The Gallery class should contain the following attributes.

Attribute	Type
galleryId	int
galleryName	String
location	String
artists	List<Artist>
GalleryRepository.java: Create an interface containing the required methods.
GalleryJpaService.java: Update the service class with logic for managing gallery data.
GalleryController.java: Create the controller class to handle HTTP requests.
GalleryJpaRepository.java: Create an interface that implements the JpaRepository interface.
Implement the following APIs.

API 1: GET /galleries
API 2: POST /galleries
API 3: GET /galleries/{galleryId}
API 4: PUT /galleries/{galleryId}
API 5: DELETE /galleries/{galleryId}
API 6: GET /galleries/{galleryId}/artists
API 7: GET /galleries/artists
API 8: POST /galleries/artists
API 9: GET /galleries/artists/{artistId}
API 10: PUT /galleries/artists/{artistId}
API 11: DELETE /galleries/artists/{artistId}
API 12: GET /artists/{artistId}/arts
API 13: GET /artists/{artistId}/galleries
API 14: GET /galleries/artists/arts
API 15: POST /galleries/artists/arts
API 16: GET /galleries/artists/arts/{artId}
API 17: PUT /galleries/artists/arts/{artId}
API 18: DELETE /galleries/artists/arts/{artId}
API 19: GET /arts/{artId}/artist
Do not modify the code in ArtGalleryApplication.java
