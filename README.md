# Blog
Tutorials and more

```cs
public class Progress : MonoBehaviour
{
    
    #region Variables
    public enum ProgressionStates { NewGame, Continue };
    public ProgressionStates currentState;

    public const string PROGRESS_SAVE_CODE = "PROGRESS";
    #endregion

    #region Singleton

    public static Progress INSTANCE;

    void Awake()
    {
        if (INSTANCE == null)
        {
            INSTANCE = this;
        }
        else
        {
            if (INSTANCE != this)
            {
                Destroy(this.gameObject);
            }
        }

    }

    #endregion
}
```
[![](https://i.imgur.com/YS9xDDr.png)](https://discord.gg/tRP76Br)[![](https://i.imgur.com/6HVUK4k.jpg)](https://www.patreon.com/)
