Just quizzing
===============================================
A simple and minimalistic quiz platform created in PHP and SQLite

Requirements
------------

- PHP 5.1.2+
- SQLite3
- a web server (Apache/Nginx/IIS/etc.)

Project Page
-----------
http://blog.claudiupersoiu.ro/just-quizzing/

Demo
----
http://claudiu-persoiu.github.io/Just-Quizzing-Server/demo/

Installation
------------

- Copy the files to the server public folder (usually *www* or *htdocs*);
- Make sure the web server have write permissions to db.info file and questions-img folder;
- Run *yourdomain/admin.php*, with user "admin" and password "admin" (without quotes);
- Delete *upgrade-db.php*

Upgrade
------

- Backup the *data* folder in a safe location;
- Overwrite the files with the new version;
- Copy the data folder back in the quiz and overwrite with your saved files;
- Make sure the web server have write permissions to *db.info* file and *questions-img* folder;
- Open *yourdomain/update-db.php* to update the database, if there aren't any issues you should see *Update complete*;
- After the update has run successfully delete *update-db.php*.

Debug
-----

If you see a black screen you can try to modify:

    ini_set('display_errors', '1');

inside *includes/config.php*.

----

DISCLAIMER

 IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.